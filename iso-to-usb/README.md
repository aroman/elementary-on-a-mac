## How to turn a Freya ISO into USB installation media

1. Download the ISO of elementary OS Freya.
2. Open **Disk Utility**.
3. Convert the ISO to DMG format:
  1. In Disk Utility, click **Images** > **Convert...**.
  2. Select the ISO and click **Convert**.
  3. Set **Image Format** to **read/write**.
  4. Click **Save**.
4. Insert your >1GB USB drive into your Mac.

  ![insert-usb](img/insert-usb.png)
5. Erase your USB drive:

  a. In Disk Utility's sidebar, select the USB drive.

  ![no-fde](img/select-usb.png)

  b. Click on the **Erase** tab.

  ![erase-tab](img/erase-tab.png)

  c. Select **MS-DOS (FAT)** from the **Format** drop-down menu.

  ![erase-tab](img/format-fat.png)

  d. Click **Erase...**.

  ![erase-button](img/erase-button.png)

  e. In the drop-down window, click "Erase".

  ![erase-confirm](img/erase-confirm.png)

6. Unmount the USB drive:

  a. In Disk Utility's sidebar, select the USB drive.

  ![no-fde](img/select-usb.png)
7. `sudo dd if=/path/to/freya.dmg of=/dev/rdiskX bs=1m` :(
