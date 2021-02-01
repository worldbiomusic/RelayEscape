# `English`
# Description
- Time Cycle which manages player's everything  

# Cycle Order
`WaitingTime` -> `MakingTime` -> `TestingTime` -> `ChallengingTime` -> `WaitingTime` -> ...(cycle)

# Features
- At the beggining of each time, goods that math the role of the RelayTime are automatically add to inventory
- Every RelayTime has its own life time, after the end of the life time, it automatically moves to the next RelayTime according to the cycle flow
- Maker can make room in MakingTime and have to clear the test for saving room to server data file and start ChallengingTime with own room
- Except for rooms with special purposes(MiniGame Room, Fun Room, empty), all rooms are guaranteed to have a existence of a Core(rule of MakingTime) and room clear certainty(rule of TestingTime)

# RelayTime Cycle Flow
![RelayTimeCycleFlow](https://github.com/worldbiomusic/RelayEscape/blob/main/imgs/RelayTimeCycleFlow.png)

# Exception
- When Maker quit the server: start ChallengingTime
-----
# RelayTime List
## [WaitingTime](WaitingTime.md)
- Time when waiter can prepare
> - Maker(`Waiter`): prepare for next Time
> - Challenger(`Waiter`): prepare for next Time

## [MakingTime](MakingTime.md)
- Time when maker can create room
> - Maker(`Maker`): make room(should put core block)
> - Challenger(`Waiter`): enjoy other rooms

## [TestingTime](TestingTime.md)
- Time when tester try to pass the room test
> - Maker(`Tester`): should clear own room for certainty
> - Challenger(`Waiter`): enjoy other rooms

## [ChallengingTime](ChallengingTime.md)
- Time when challenger try to find the core
> - Maker(`Viewer`): just watch
> - Challenger(`Challenger`): try to find the core
---------------------------------------------------------------------------------------------------------------------
---------------------------------------------------------------------------------------------------------------------
---------------------------------------------------------------------------------------------------------------------
# `Korean`
# 설명
- 유저의 모든걸 관리하는 시간사이클

# 사이클 순서
`WaitingTime` -> `MakingTime` -> `TestingTime` -> `ChallengingTime` -> `WaitingTime` -> ...(cycle)

# 특징
- 매 타임이 시작될 때마다 `해당 타임의 역할`에 맞는 굿즈가 자동으로 인벤토리에 지급됩니다
- 모든 시간사이클은 각자의 수명시간을 가지고 있습니다. 수명시간이 다 한 후에는 사이클흐름에 맞게 다음 시간사이클로 자동으로 넘어갑니다
- 룸은 MakingTime때 만들고, TestingTime때 만든 본인의 룸을 무조건 클리어해야 룸이 저장되고 ChallengingTime이 시작됩니다
- 특별한 목적을 가진 룸(MiniGame Room, Fun Room, empty)을 제외한 모든 룸은 의`코어의 존재`(MakingTime의 규칙)와, `룸 클리어 확실성`(TestingTime의 규칙)이 보장되어 있습니다

# 릴레이타임 사이클 흐름
![RelayTimeCycleFlow](https://github.com/worldbiomusic/RelayEscape/blob/main/imgs/RelayTimeCycleFlow.png)

# 예외상황
- 메이커가 서버를 나갈때: ChallengingTime 
-----
# RelayTime List
## [WaitingTime](WaitingTime.md)
- 모든 플레이어가 준비를 하는 타임
> - Maker(`Waiter`): 다음 시간 준비
> - Challenger(`Waiter`): 다음 시간 준비

## [MakingTime](MakingTime.md)
- 메이커가 룸을 만드는 타임
> - Maker(`Maker`): 룸을 만듬(코어 놓아야 함)
> - Challenger(`Waiter`): 서버 즐기기

## [TestingTime](TestingTime.md)
- 테스터가 만든 룸을 테스트하는 타임
> - Maker(`Tester`): 확실성을 위해서 테스트를 성공해야 함
> - Challenger(`Waiter`): 서버 즐기기

## [ChallengingTime](ChallengingTime.md)
- 도전자들이 도전하는 타임
> - Maker(`Viewer`): 관전
> - Challenger(`Challenger`): 코어를 찾기



