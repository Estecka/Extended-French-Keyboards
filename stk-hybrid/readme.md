# French Qwazerty Hybrid

Motivated by the same reasoning as the [French Qwerty](../stk-wasd/readme.md) layout.

This is an attempt at making a keyboard that would be treated as Azerty when typewriting, but as Qwerty when gaming.

Whilst it was successful in _some_ contexts, it can also be very unpredictable in many other ones, so I would not actually recommend using it, except for study or as a negative example.

## How ?

While experimenting with MKLC, I figured that keys have two independent properties: the **keycode**, and the **written character**. It's technically possible for a key to send the `Z` keycode, but write the `W` character; and this is exactly what this layout does.

Keycode-wise, this keyboard is layed out like a Qwerty, so that the traditional movement keys send video-games are the `WASD` key codes. But when typewriting, it is layed out as an Azerty.

Does it work as intended ? In some games yes, (most notably, Unity3D games); even within such games, character controls succesfully receive the WASD layout, while text-editing preserves the Azerty layout. Alas, some other games appear to ignore the keycode in some way, and will treat the layout as pure Azerty (E.g: Totally Accurate Battlegrounds), defeating the point of using this layout in the first place.

Where this layout breaks the most however, is in daily life applications. The traditional keyboard shortcuts (`Ctrl+Z`, `Ctrl+A`, etc) used in pretty much every software seem to be bound to the keycodes, and so to the Qwerty side of the layout. It is very confusing to try and hit `Ctrl+Z` and ending up quitting the app because it thought you meant `Ctrl+W`.