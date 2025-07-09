

# Caldera keymap

[Caldera](https://christianselig.com/2024/07/caldera-keyboard/) is a very beautifully designed split keyboard by Christian Selig. It is also not the most ergonomic keyboard as it doesn't have a thumb cluster.

I find that only the 2 bottom keys closest to the thumbs from the bottom row are comfortable to use so I assigned them the most used keys: `SHIFT`, `SPACE`, `RETURN`, and `BACKSPACE`. Having only 4 "thumb keys" makes that dedicating a single keys a layer very taxing, so I strongly recomend using zmk's [tap dance](https://zmk.dev/docs/keymaps/behaviors/tap-dance) and [hold tap](https://zmk.dev/docs/keymaps/behaviors/hold-tap) functionalities.

In my keymap:

- `LYR1/F` = Hold tap F (`&lt 1 F`): Layer 1 is activated when F holded.
- `LYR2/RET` = Hold tap Enter (`&lt 2 RET`): Layer 2 is activated when F holded.
- `TD_SHF` = Tap Dance: tap once Left Shift, tap twice for Caps Lock


**Default Layer (Layer 0)**

```
,-----------------------------------------.      ,------------------------------------------.
|  `   |  1   |  2  |  3   |  4    |  5   |      |   6   |  7   |  8   |  9   |  0   | DEL  |
|------+------+-----+------+-------+------|      |-------+------+------+------+------+------|
| ESC  |  Q   |  W  |  E   |  R    |  T   |      |   Y   |  U   |  I   |  O   |  P   |  =   |
|------+------+-----+------+-------+------|      |-------+------+------+------+------+------|
| TAB  |  A   |  S  |  D   | L1/F  |  G   |      |   H   |  J   |  K   |  L   |  ;   |  -   |
|------+------+-----+------+-------+------|      |-------+------+------+------+------+------|
|TD_SHF|  Z   |  X  |  C   |  V    |  B   |      |   N   |  M   |  ,   |  .   |  /   |  _   |
|------+------+-----+------+-------+------|      |-------+------+------+------+------+------|
| LCTRL| LGUI |  \  | LALT | LSHFT | SPACE|      |L2/RET | BSPC | RALT | GLOBE| RGUI | LCTRL|
`-----------------------------------------'      '------------------------------------------'
```

**Symbol Layer (Layer 1)**

```
,-----------------------------------------.      ,------------------------------------------.
|      |      |      |      |      |      |      |      |      |      |      |      |       |
|------+------+------+------+------+------|      |------+------+------+------+------+-------|
|      |BRI_UP|BRI_DN|      |      |      |      |  @   |  [   |  "   |  ]   |  &   |  $    |
|------+------+------+------+------+------|      |------+------+------+------+------+-------|
|      | PREV |  PP  | NEXT |      |      |      |  #   |  (   |  '   |  )   |  +   |  ~    |
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

## Idea behind the layers setup

- Symbols layer

Holding `F` makes all the symbols I need available on the right side and the few media controls I normally use on my left side next to `F`.

This feels more comfortable that moving my right index finger to other key, as it is naturally resting on top of the `F` key. I don't feel any advantage of using both keyboard sides for symbols in this keyboard as there are plenty of keys in one side.

I tried using `SPACE` as hold tap key, but it creates "chunky" typing experience. The `hold tap` creates a micro delay in the key that is mostly unperceivable unless you are tapping the key constantly, which is the case with `SPACE`.

- Numbers and arrow layer

Holding `ENTER` creates a numpad on my left side. I've never used a numpad in my life before, so I don't mind having it in at my left hand. For some OCD reason I like to have it ordered 1 to 9 instead of 9 to 1.

It also creates arrow keys in `JKIL`, very close to the home row were the hand rest. They are arrow keys, not the `HJKL` directional movement keys as in vim fashion. `HOME` and `END` are in the left and right to the arrows to go all the way to the left and al the way to the right respectively.

I tried using `J` as hold tap key for symmetry with the other hold key `F`, but then I wouldn't be able to use this layer for the arrow keys. Creating an extra layer to simply use `J` is overcompling things as holding `ENTER` is equally comfy.
