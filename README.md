walter-karabiner-config
=======================

Karabiner-Elements uses a single config file:

    ~/.config/karabiner/karabiner.json

Copy the designated json to the "global" karabiner.json

warning: copying the wrong json may mess up / confuse your keyboard !

* `neo1.json` is for a Japanese macbook neo:
  * builtin keyboard is Japanese; karabiner keyboard setting is JIS
    * this is such that the builtin keyboard should always work normally
    * ABC and Japanese characters key are mapped to (an additional) left + right Command key
    * caps lock is mapped to left control
  * complex rules for external keyboards;
    * external keyboards are (implicitly) expected to be ANSI
    * ANSI keys are mapped "back" to JIS driver
  * Option+ArrowUp, Option+ArrowDown are mapped to PageUp, PageDown for all keyboards
  * caps lock is mapped to left control (now for all keyboards)
  * note: use `US` keyboard language setting in macOS
    * note: `US International PC` produces a weird/broken tilde key (it's a tilde accent rather than a tilde character)

