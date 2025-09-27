# My own Malicious Python Samples

### WARNING: I AM NOT RESPONSIBLE FOR ANY ACCIDENTAL DAMAGE ON ANYBODY'S COMPUTER!
---

### bsod.py
This is a VERY simple BSOD-on-login script that REQUIRES INTERNET.
It simply creates a .bat which runs a PowerShell script hidden running 
[Peewpw's invoke BSOD script ](https://github.com/peewpw/Invoke-BSOD/). (thank you Peewpw)

To remove, simply start up via Safety mode, open Explorer - and go to ``shell:startup`` - then delete ``dsaksdbanladlkdnsad.bat``

### cursor.py
This is a silly Malware-like demo that moves the cursor erratically when the script is pressed. What it does is it invokes ``user32.dll`` calls to press ``Win+R``, open ``notepad.exe``, and type a very corny message, and moving the cursor everywhere. (``You are no longer in control.``)

To remove, ``Alt+Tab`` to the python shell and press ``Alt+F4``.

### errors.py

This is a fake Windows Critical Error generator that creates errors that say stuff such as:

*Critical memory management failure detected (0x0000011A). Save your work immediately and restart your computer. *

It is more of scareware, and can be easily stopped by ``Alt+Tab``ing to the python shell and pressing ``Alt+F4``.

### Forkbomb.py

It is more of a snail; but it works fine! What it does is it opens itself and then forever calculates random numbers between 1 and 100 forever.

To remove, just restart your computer.

### GDIfunnies.py

This is one of my favourites! It invokes ``user32.dll``, ``gdi32.dll``, ``kernel32.dll``, and ``winmm.dll`` to create a GDI malware effect. Admittedly, yes, I did use a bit of Artificial Intelligence - however this is because I barely even know how to use ``ctypes`` let alone ``gdi32.dll``.

It causes a screen tear effect, random error icons popping up, random sounds, and consumes **ALOT** of system resources.

To remove, ``Alt+Tab`` to the python shell and press ``Alt+F4``, then delete all the ``.tmp`` files (they are to make the RAM clogged).

### Test.py

It repeatedly asks for UAC until it has admin, and then gives you a GUI with some buttons. Try to close it, you lose. Press one and you have a chance of losing. If you lose, it forcefully removes the ``C:\`` partition and tries to delete it out. Then it forcefully restarts your computer with ``shutdown -r -f -t 0``.

To remove, restart your computer before pressing any buttons.

### UAC.py

It attempts to bypass UAC via some attempts. Nothing bad. Just tests you.
