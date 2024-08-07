# beatmania IIDX 30 RESIDENT
<img src="/img/iidx30-31/resident.png">

!!! danger "Please make sure you downloaded your data from an appropriate source.<br>This guide is unable to troubleshoot any problems related to bad or poorly managed data."
    
---
### About ea3-config.xml

!!! tip ""

    The `ea3-config.xml` file is located inside the `prop` folder. 

    Below is an explanation on what different sections of this file do.

    The following lines change the PCBID and HARDID that your system reports to your e-amusement server.  
    There is ^^**no need to manually change this**^^ as `spice2x` will do it for us.
    
    ```xml
    <pcbid __type="str">00010203040506070809</pcbid>
    <hardid __type="str">00010203040506070809</hardid>
    ```

    The following line determines what version of the game you are running.  
    ^^**You should never change this**^^. It should always say `LDJ`.

    ```xml
    <model __type="str">LDJ</model>
    ```

	The following line determines the game's region.
	^^**You should never change this**^^. As you can change the language in-game.

	```xml
	<dest __type="str">J</dest>
	```

    ^^**You should never change this**^^. It should always say `A` for Epolis.

    ```xml
    <rev __type="str">A</rev>
    ```

    The following line determines your datecode.  
    ^^**Always keep it up to date**^^ with your game's current version.

    ```xml
    <ext __type="str">2024052100</ext>
    ```

    The following line determine what remote service URL `spice2x` is supposed to connect to.  
    There is ^^**no need to manually change this**^^ as `spice2x` will do it for us.

	```xml
	<services __type="str">http://localhost:8083</services>
    ```