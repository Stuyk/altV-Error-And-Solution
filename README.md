# altV-Error-And-Solution
A simple README file with a handful of error messages and solutions.

---

## Client Errors

### Basic Troubleshooting for Clients (TheBloodyScreen)

1. A CLEAN gta installation. Yes we know there are mods you might not want to live without but those can be the reason alt:V doesn't work.

2. Make sure you're running on the latest version of gta!
SC users who have problems updating: Make sure "rivatuner statistics server" is not running!

3. Run as Admin. This seems to be one of the most consistent solutions. (I myself have to do this)

4. Make sure you have "Microsoft Visual C++ 2017 Redistributable" installed. 

5. Only use ascii characters in your alt:V path.

6. Try keeping the path to alt:V as short as possible. (C:/bla/blubb/blib/stuff/things/altv.exe is not a good idea)

7. Avoid putting alt:V on your desktop.

8. **Don't run Windows 7.** If you decide to do this anyway you need update KB2670838 to run alt:V. Even then it's not guarenteed that the client will start. Just upgrade to Windows 10 already.

9. If the Steam version is stuck on "Load alt:V Client", try killing the Steam process(es). (Also try and remove Steam from autostart.)
10. Delete RageMP files from your GTA directory. alt:V also provides a .bat file that removes anything RAGE:MP related.
See the attachments in the following [thread](https://forum.altv.mp/topic/30-troubleshooting/)

### Failed to fetch updates.

This is normally an error that occurs when your connection is interrupted while updating the alt:V client. That or the CDN is having issues. This is a timing based error and it just so happens you're downloading at a bad time.

### Config parse error:key expected

If you have manually edited your altv.cfg for your client you will run into this problem. Download a new copy of alt:V to restore your client.

### Mouse Frozen, Frozen Input, Can't Click Anything

Update your mouse input to Raw Input and de-activate your controller. This can be done manually by editing a configuration file for GTA:V or booting into single player to change the settings.

### Something else hooked DirectX context. Try to shutdown programs that can do it... (Riva Tuner, Fraps, etc.)

This error message should be self explanatory but for some of you it is not. Turn off anything that gives you an FPS overlay. Anything that will record the game. It's screwing up the boot process for alt:V.


### Oops, game crashed. Do you want to save a crashdump?

Save the dump and upload it to the #support section of Discord. This is useful information for the alt:V developers. Try joining the same server again. This is just a standard issue crash and there is no fix for it.

## Server Errors

### [Error] Failed to load module modules/node-module.dll
### Module uses incompatible SDK version(v16) while v17 is required

This only occurs when the version somehow becomes corrupted or is not done fully done building the latest version. The simplest solution to this is manually download the latest version of server files.

### Thread 1 "altv-server" received signal SIGSEGV, Segmentation fault.

There is no perfect solution to this. This error is unique to alt:V and only happens once in a while. A common thing that is recommend is to turn on core dumps for linux. Then pass the core dumps to developers. Refer to this: https://linux-audit.com/understand-and-configure-core-dumps-work-on-linux/

### Connection failed: Server error WRONG_PASSWORD

Either the server has a password OR the server does not have a password and you just need to type reconnect with two spaces after. Here's an example of how that looks: `reconnect  `. Note the spaces AFTER reconnect.

### Failed to write into a file: altv-new.exe

This has to do with incorrect permissions on windows to write to the directory where you extracted it. There are two places you should **absolutely not** install alt:V. Do **not** install it on the desktop. Do **not** install it where GTA:V is located. Do install it on another drive, in your documents, or anywhere else but the two places that are listed here.

### libatomic error

This is a linux specific error. Just run the following command `apt-get install libatomic`.




