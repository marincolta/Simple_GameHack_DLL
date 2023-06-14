# Simple_GameHack_DLL
This code represents a DLL written for a game. It demonstrates how to manipulate memory addresses to implement various hacks, such as infinite health, unlimited ammo, and removing recoil.
<picture>
 <source media="(prefers-color-scheme: dark)" srcset="https://i.pinimg.com/originals/c9/19/fc/c919fc265985a7d42e6677e53dd05b0c.jpg">

</picture>


We made this DLL which is good for the injector.
IN the first part of the code we use the function "AllocCOnsole" to check if the DLL was injected mostly succesfully.
After that by using the function GetModuleHandle we get the handle to the game, which we also
recasting to uintptr_t and futhermor we call it with Null so we could get the adress  of the exe module.

We use the function "GetAsyncKeyState(key) & 1" function to check if the given button was pressed, we check if the current button was pressed thanks to "& 1"

We got the stack for example "\x50\x8D\x4C\x24\x1C\x51\x8B\xCE\xFF\xD2" thanks to CH (Cheat Engine) by looking at the bytes of some functions / memory addresses. (SO you should have knowledge in Cheat Engine too but i will leave a photo too")


