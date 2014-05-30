## How to turn an Isis ISO into USB installation media

### Using the command line

1. Download the ISO. Let's assume it's in `~/Downloads`.
2. Convert the ISO to DMG format: `hdiutil convert -format UDRW -o isis elementaryos-unstable-amd64.20140529.iso`.
3. Insert your >1GB USB drive into your Mac.
4. Determine and make note of the mount point of your USB drive.

### Using Disk Utility

1. Download the ISO. Let's assume it's in `~/Downloads`.
2. Open **Disk Utility**.
3. Convert the ISO to DMG format:
  1. In Disk Utility, click **Images** > **Convert...**.
  2. Select the ISO and click **Convert**.
  3. Set **Image Format** to **read/write**.
  4. Click **Save**.
4. Insert your >1GB USB drive into your Mac.

  ![insert-ursb](img/insert-usb.png)
5. Erase your USB Drive:

  a. In Disk Utility's sidebar, select the USB Drive.

  ![no-fde](img/select-usb.png)

  b. Click on the **Erase** tab.

  ![erase-tab](img/erase-tab.png)

  c. Select **MS-DOS (FAT)** from the **Format** drop-down menu.

  ![erase-tab](img/format-fat.png)

  d. Click **Erase...**.

  ![erase-button](img/erase-button.png)

  e. In the drop-down window, click "Erase".

  ![erase-confirm](img/erase-confirm.png)

6. Unmount the USB Drive:

  a. In Disk Utility's sidebar, select the USB Drive.

  ![no-fde](img/select-usb.png)