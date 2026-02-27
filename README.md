# Caldera keymap

[Caldera](https://christianselig.com/2024/07/caldera-keyboard/) is a very beautifully designed split keyboard by Christian Selig.

It is also not the most ergonomic keyboard as it doesn't have a thumb cluster. I find that only the 2 bottom keys closest to the thumbs from the bottom row are comfortable to use so I assigned them the most used keys: `BACKSPACE`, `SPACE`, `RETURN`, and `SYSTEM`.

Having only 4 "thumb keys" makes that dedicating a single keys a layer very taxing, so I strongly recomend using zmk's [tap dance](https://zmk.dev/docs/keymaps/behaviors/tap-dance) and [hold tap](https://zmk.dev/docs/keymaps/behaviors/hold-tap) functionalities.

In my keymap:

- `LYR1/F` = Hold tap F (`&lt 1 F`): Layer 1 is activated when F holded.
- `LYR2/RET` = Hold tap Enter (`&lt 2 RET`): Layer 2 is activated when F holded.
- `TD_SHF` = Tap Dance: tap once Left Shift, tap twice for Caps Lock

**Default Layer (Layer 0)**

```
,-----------------------------------------.      ,------------------------------------------.
|  ESC |  1   |  2  |  3   |  4    |  5   |      |   6   |  7   |  8   |  9   |  0   | DEL  |
|------+------+-----+------+-------+------|      |-------+------+------+------+------+------|
|   `  |  Q   |  W  |  E   |  R    |  T   |      |   Y   |  U   |  I   |  O   |  P   |  =   |
|------+------+-----+------+-------+------|      |-------+------+------+------+------+------|
| TAB  |  A   |  S  |  D   | L1/F  |  G   |      |   H   |  J   |  K   |  L   |  ;   |  -   |
|------+------+-----+------+-------+------|      |-------+------+------+------+------+------|
|TD_SHF|  Z   |  X  |  C   |  V    |  B   |      |   N   |  M   |  ,   |  .   |  /   | RSHFT|
|------+------+-----+------+-------+------|      |-------+------+------+------+------+------|
| LCTRL| LGUI |  \  | LALT | BSPC | SPACE |      |L2/RET | RGUI | RALT | GLOBE| RGUI | RCTRL|
`-----------------------------------------'      '------------------------------------------'
```

**Symbol Layer (Layer 1)**

```
,-----------------------------------------.      ,------------------------------------------.
|      |      |      |      |      |      |      |      |      |      |      |      |       |
|------+------+------+------+------+------|      |------+------+------+------+------+-------|
|      |BRI_UP|BRI_DN|      |      |      |      |  @   |  [   |  "   |  ]   |  &   |  $    |
|------+------+------+------+------+------|      |------+------+------+------+------+-------|
|      | PREV |  PP  | NEXT |      |      |      |  #   |  (   |  '   |  )   |  ^   |  ~    |
|------+------+------+------+------+------|      |------+------+------+------+------+-------|
|      |      |      |      |      |      |      |  !   |  {   |  *   |  }   |  %   |  |    |
|------+------+------+------+------+------|      |------+------+------+------+------+-------|
|      |      |      |      |      |      |      |      |      |      |      |      |       |
`-----------------------------------------'      '------------------------------------------'

```

**Numbers Layer (Layer 2)**

```
,-----------------------------------------.      ,-----------------------------------------.
|      |      |      |      |      |      |      |      |      |      |       |      |      |
|------+------+------+------+------+------|      |------+------+------+-------+------+------|
|      |      |  1   |  2   |  3   |      |      |      |      | UP   |       |      |      |
|------+------+------+------+------+------|      |------+------+------+-------+------+------|
|      |      |  4   |  5   |  6   |  0   |      | HOME | LEFT | DOWN | RIGHT | END  |      |
|------+------+------+------+------+------|      |------+------+------+-------+------+------|
|      |      |  7   |  8   |  9   |      |      |      |      |      |       |      |      |
|------+------+------+------+------+------|      |------+------+------+-------+------+------|
|      |      |      |      |      |      |      |      |      | BT0  |  BT1  | BT2  |BT_CLR|
`-----------------------------------------'      '------------------------------------------'

```

## [Why this layers setup?](https://gist.github.com/pipegalera/96ebbe37e71e2c9030cf3b9d0725b4fb)


