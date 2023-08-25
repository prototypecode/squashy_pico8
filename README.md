# Squashy Pico-8

[Demo Game](https://prototypecode.itch.io/squashy-pico-8)

---

## Step 1: Paddle

### Pg. 0

```lua

--paddle
padx = 52
pady = 122
padw = 24
padh = 4

function movepaddle()
  if btn(0) then
    padx -= 3
  elseif btn(1) then
    padx += 3
  end
end

function _update()
  movepaddle()
end

function _draw()
  --clear the screen
  rectfill(0, 0, 128, 128, 3)

  --draw the paddle
  rectfill(padx, pady, padx + padw, pady + padh, 15)
end

```

---

[Step 2: Ball](step_2.md)

---
