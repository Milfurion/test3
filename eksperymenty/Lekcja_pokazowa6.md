### @hideIteration false 
### @flyoutOnly 1
### @explicitHints 1


# Super linia z haszem 
## Step 1
Super ekstra lekcja pokazowa

```tutorial
let y = 0
let y2 = 0
player.onChat("wieża", function () {
    agent.teleport(world(-46, 4, 40), NORTH)
    agent.setItem(STONE_BRICKS, 64, 1)
    agent.setSlot(1)
    for (let index = 0; index < 5; index++) {
        agent.setItem(STONE_BRICKS, 64, 1)
        agent.setAssist(PLACE_ON_MOVE, true)
        agent.move(FORWARD, 25)
        agent.turn(LEFT_TURN)
        agent.setItem(STONE_BRICKS, 64, 1)
        agent.move(FORWARD, 25)
        agent.turn(LEFT_TURN)
        agent.setItem(STONE_BRICKS, 64, 1)
        agent.move(FORWARD, 25)
        agent.turn(LEFT_TURN)
        agent.setItem(STONE_BRICKS, 64, 1)
        agent.move(FORWARD, 24)
        agent.setAssist(PLACE_ON_MOVE, false)
        agent.setItem(STONE_BRICKS, 64, 1)
        agent.move(UP, 1)
        agent.place(DOWN)
        agent.move(FORWARD, 1)
        agent.turn(LEFT_TURN)
        // test
    }
    agent.teleport(world(-45, 6, 36), WEST)
    oknox3()
    agent.teleport(world(-45, 6, 21), WEST)
    oknox3()
    agent.teleport(world(-45, 6, 28), WEST)
    agent.destroy(FORWARD)
    agent.move(UP, 1)
    agent.destroy(FORWARD)
    agent.move(RIGHT, 1)
    agent.destroy(FORWARD)
    agent.move(DOWN, 1)
    agent.destroy(FORWARD)
    y = 9
    blocks.fill(
    RED_WOOL,
    world(-47, 4, 39),
    world(-70, 4, 16),
    FillOperation.Replace
    )
    for (let index = 0; index < 50; index++) {
        blocks.clone(
        world(-45, 4, 41),
        world(-72, 9, 14),
        world(-72, y, 14),
        CloneMask.Replace,
        CloneMode.Normal
        )
        y += 5
        loops.pause(100)
    }
    loops.pause(1000)
    blocks.replace(
    GLASS,
    STONE_BRICKS,
    world(-45, 6, 36),
    world(-47, 255, 19)
    )
    blocks.fill(
    AIR,
    world(-23, 4, 24),
    world(-19, 9, 11),
    FillOperation.Replace
    )
})
player.onChat("wyjście", function () {
    blocks.fill(
    GRASS,
    world(-24, 1, 27),
    world(-24, 1, 10),
    FillOperation.Replace
    )
    blocks.fill(
    AIR,
    world(-24, 4, 27),
    world(-24, 20, 10),
    FillOperation.Replace
    )
})
player.onChat("usuń", function () {
    y = 4
    y2 = 35
    for (let index = 0; index < 15; index++) {
        blocks.fill(
        AIR,
        world(-45, y, 41),
        world(-72, y2, 14),
        FillOperation.Replace
        )
        y += 20
        y2 += 20
    }
})
loops.forever(function () {
    blocks.clone(
    world(4, 4, -10),
    world(4, 10, 9),
    world(3, 4, -10),
    CloneMask.Replace,
    CloneMode.Normal
    )
    blocks.clone(
    world(-24, 4, -11),
    world(2, 10, -11),
    world(-24, 4, -10),
    CloneMask.Replace,
    CloneMode.Normal
    )
    blocks.clone(
    world(-25, 4, 9),
    world(-25, 10, -9),
    world(-24, 4, -9),
    CloneMask.Replace,
    CloneMode.Normal
    )
    loops.pause(200)
    blocks.clone(
    world(5, 4, -10),
    world(5, 10, 9),
    world(3, 4, -10),
    CloneMask.Replace,
    CloneMode.Normal
    )
    blocks.clone(
    world(-24, 4, -12),
    world(2, 10, -12),
    world(-24, 4, -10),
    CloneMask.Replace,
    CloneMode.Normal
    )
    blocks.clone(
    world(-26, 4, 9),
    world(-26, 10, -9),
    world(-24, 4, -9),
    CloneMask.Replace,
    CloneMode.Normal
    )
    loops.pause(200)
    blocks.clone(
    world(6, 4, -10),
    world(6, 10, 9),
    world(3, 4, -10),
    CloneMask.Replace,
    CloneMode.Normal
    )
    blocks.clone(
    world(-24, 4, -13),
    world(2, 10, -13),
    world(-24, 4, -10),
    CloneMask.Replace,
    CloneMode.Normal
    )
    blocks.clone(
    world(-27, 4, 9),
    world(-27, 10, -9),
    world(-24, 4, -9),
    CloneMask.Replace,
    CloneMode.Normal
    )
    loops.pause(200)
})
player.onChat("tp", function () {
    agent.teleportToPlayer()
})
player.onChat("uwolnij", function () {
    blocks.fill(
    AIR,
    world(-23, 4, 24),
    world(-19, 9, 11),
    FillOperation.Replace
    )
})
player.onChat("zburz most", function () {
    agent.teleport(world(-16, 12, 174), SOUTH)
    agent.setItem(REDSTONE_TORCH, 64, 4)
    agent.setSlot(4)
    agent.place(FORWARD)
    agent.teleport(world(-16, 10, 158), NORTH)
    agent.place(FORWARD)
    agent.teleport(world(-13, 7, 160), SOUTH)
    for (let index = 0; index < 13; index++) {
        agent.destroy(FORWARD)
        agent.move(FORWARD, 1)
    }
    agent.turn(LEFT_TURN)
    agent.move(FORWARD, 3)
    agent.turn(LEFT_TURN)
    for (let index = 0; index < 13; index++) {
        agent.destroy(FORWARD)
        agent.move(FORWARD, 1)
    }
    agent.turn(LEFT_TURN)
    agent.move(FORWARD, 3)
    agent.turn(LEFT_TURN)
    agent.move(DOWN, 1)
    for (let index = 0; index < 13; index++) {
        agent.destroy(FORWARD)
        agent.move(FORWARD, 1)
    }
    agent.turn(LEFT_TURN)
    agent.move(FORWARD, 3)
    agent.turn(LEFT_TURN)
    for (let index = 0; index < 13; index++) {
        agent.destroy(FORWARD)
        agent.move(FORWARD, 1)
    }
    agent.turn(LEFT_TURN)
    agent.move(FORWARD, 2)
    agent.turn(LEFT_TURN)
    for (let index = 0; index < 13; index++) {
        agent.destroy(FORWARD)
        agent.move(FORWARD, 1)
    }
    agent.turn(LEFT_TURN)
    agent.move(FORWARD, 1)
    agent.turn(LEFT_TURN)
    for (let index = 0; index < 13; index++) {
        agent.destroy(FORWARD)
        agent.move(FORWARD, 1)
    }
    agent.turn(LEFT_TURN)
    agent.move(FORWARD, 2)
    agent.turn(LEFT_TURN)
    agent.move(DOWN, 1)
    for (let index = 0; index < 13; index++) {
        agent.destroy(FORWARD)
        agent.move(FORWARD, 1)
    }
    agent.turn(LEFT_TURN)
    agent.move(FORWARD, 3)
    agent.turn(LEFT_TURN)
    for (let index = 0; index < 13; index++) {
        agent.destroy(FORWARD)
        agent.move(FORWARD, 1)
    }
    agent.turn(LEFT_TURN)
    agent.move(FORWARD, 2)
    agent.turn(LEFT_TURN)
    for (let index = 0; index < 13; index++) {
        agent.destroy(FORWARD)
        agent.move(FORWARD, 1)
    }
    agent.turn(LEFT_TURN)
    agent.move(FORWARD, 1)
    agent.turn(LEFT_TURN)
    for (let index = 0; index < 13; index++) {
        agent.destroy(FORWARD)
        agent.move(FORWARD, 1)
    }
})
function oknox3 () {
    agent.destroy(FORWARD)
    agent.move(UP, 1)
    agent.destroy(FORWARD)
    agent.move(RIGHT, 1)
    agent.destroy(FORWARD)
    agent.move(DOWN, 1)
    agent.destroy(FORWARD)
    agent.move(RIGHT, 1)
    agent.destroy(FORWARD)
    agent.move(UP, 1)
    agent.destroy(FORWARD)
}
player.onChat("zbuduj most", function () {
    blocks.fill(
    STONE_BRICKS,
    world(-4, 3, 160),
    world(-15, 3, 160),
    FillOperation.Replace
    )
    blocks.fill(
    STONE_BRICKS,
    world(-7, 3, 173),
    world(-15, 3, 173),
    FillOperation.Replace
    )
    agent.teleport(world(-13, 5, 160), SOUTH)
    agent.setItem(STONE_BRICKS_SLAB, 64, 1)
    agent.setItem(STONE_BRICKS, 64, 2)
    agent.setItem(ACACIA_FENCE, 64, 3)
    agent.move(FORWARD, 1)
    for (let index = 0; index < 2; index++) {
        agent.setSlot(2)
        agent.setAssist(PLACE_ON_MOVE, true)
        agent.move(FORWARD, 1)
        agent.move(UP, 1)
        agent.move(FORWARD, 9)
        agent.move(DOWN, 1)
        agent.move(FORWARD, 2)
        agent.setAssist(PLACE_ON_MOVE, false)
        agent.turn(LEFT_TURN)
        agent.move(FORWARD, 3)
        agent.turn(LEFT_TURN)
        agent.move(FORWARD, 1)
    }
    agent.move(LEFT, 1)
    agent.move(FORWARD, 1)
    for (let index = 0; index < 2; index++) {
        agent.setSlot(1)
        agent.setAssist(PLACE_ON_MOVE, true)
        agent.move(FORWARD, 1)
        agent.setSlot(2)
        agent.move(FORWARD, 1)
        agent.setAssist(PLACE_ON_MOVE, false)
        agent.move(UP, 1)
        agent.setSlot(1)
        agent.setAssist(PLACE_ON_MOVE, true)
        agent.move(FORWARD, 8)
        agent.setAssist(PLACE_ON_MOVE, false)
        agent.setSlot(2)
        agent.place(DOWN)
        agent.setSlot(1)
        agent.move(FORWARD, 1)
        agent.place(DOWN)
        agent.turn(LEFT_TURN)
        agent.move(FORWARD, 1)
        agent.turn(LEFT_TURN)
        agent.move(DOWN, 1)
    }
    agent.move(UP, 1)
    agent.move(RIGHT, 1)
    for (let index = 0; index < 2; index++) {
        agent.setSlot(3)
        agent.move(BACK, 1)
        agent.place(FORWARD)
        agent.move(UP, 1)
        agent.move(FORWARD, 1)
        agent.setAssist(PLACE_ON_MOVE, true)
        agent.move(FORWARD, 12)
        agent.setAssist(PLACE_ON_MOVE, false)
        agent.move(DOWN, 1)
        agent.place(BACK)
        agent.move(BACK, 1)
        agent.turn(LEFT_TURN)
        agent.move(FORWARD, 3)
        agent.turn(LEFT_TURN)
    }
    agent.teleport(world(-16, 10, 158), NORTH)
    agent.destroy(FORWARD)
    agent.teleport(world(-16, 12, 174), SOUTH)
    agent.destroy(FORWARD)
})


```


# Super linia z haszem 
## Step 2
A teraz własny kod

```blocks
player.onChat("Hej", function () {
    player.say("A dzień dobry, dzień dobry :)")
})


```





