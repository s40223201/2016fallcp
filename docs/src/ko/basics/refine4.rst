
단계적 정제: 4부
===================

여러분 대부분 알아내셨듯이, 토큰을 내려 놓은 후에 너무나도 서둘러서 리보그에게 앞으로 전진하게 명령을 한 것이다. 
앞으로 움직이기 전에 벽이 있는지를 확인하는 단계가 필요하다. 여기에 문제에 대한 해답이 있다::

    put()
    if not front_is_clear():
        turn_left()
    move()
    while not object_here():
        if right_is_clear():
            turn_right()
            move()
        elif front_is_clear():
            move()
        else:
            turn_left()

.. topic:: 시도해 보기!

    지금 당장 테스트해보고 정상적으로 작동하는지 확인한다. 
    이 프로그램이 동작할 것 같지 않는 상황을 상상할 수 있나요?

정교화: 5부
===================

**Around 4** 세상을 고려한다.

.. topic:: 시도해 보기!

    앞서 작성한 프로그램이 작동하나요?

아마도 생각하듯이, 이 프로그램은 작동하지 않는다. 
만약 시도하지 않았다면 정말 시도해봐야 합니다.
정상적으로 작동시키기 위해서, 방금 전에 추가한 ``while`` 명령문을 ``if`` 명령문으로 바꿀 필요가 있다. 시도해 보세요!
