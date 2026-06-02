walter-karabiner-config
=======================

Karabiner-Elements uses a single config file:

    ~/.config/karabiner/karabiner.json

Copy the designated json to the "global" karabiner.json
or better: import the json file into Karabiner settings.

warning: copying the wrong json may mess up / confuse your keyboard !

* `neo1.json` is for a Japanese macbook neo:
  * builtin keyboard is Japanese; karabiner keyboard setting is JIS
    * this is such that the builtin keyboard should always work normally
    * ABC and Japanese characters key are mapped to (an additional) left and
      right Command key
    * caps lock is mapped to left control
  * complex rules for external keyboards;
    * external keyboards are (implicitly) expected to be ANSI
    * ANSI keys are mapped "back" to JIS driver
  * Option+ArrowUp, Option+ArrowDown are mapped to PageUp, PageDown
    for all keyboards
  * caps lock is mapped to left control (now for all keyboards)
  * note: use `US` keyboard language setting in macOS
    * note: `US International PC` produces a weird/broken tilde key
      (it's a tilde accent rather than a tilde character)

* `ext-ansi-jis.json` is for an external ANSI keyboard connected to a computer
  with JIS driver

* `rkr65-dvorak-jis.json` is for (specifically) the RK-R65 keyboard with
  dvorak layout to a computer that has a JIS driver.
  Note: I'm using a customized RK-R65 with the keys physically rearranged
  to dvorak layout, while the firmware still acts like US ANSI.
  Change vendor id / product id in the json for other brands of keyboards.
  Choose US layout in macOS, Karabiner will remap to dvorak.

* `keychron-k1-us-ansi-dvorak.json` is a dvorak layout specifically for the
  keychron K1 wireless keyboard. It is a US ANSI keyboard (use the ANSI driver)
  with physically rearranged keys.
  Change vendor id / product id in the json for other brands of keyboards.
  Choose US layout in macOS, Karabiner will remap to dvorak.
