# Archao SDDM Theme

This is the Archao theme for the SDDM display manager.

## Installation

1.  **Copy the theme files:** Copy the entire directory containing this `README.md` file (e.g., `archao-sddm`) to the SDDM theme directory.  The standard location is `/usr/share/sddm/themes/`. You might need root privileges to do this.

    ```bash
    sudo cp -r archao-sddm /usr/share/sddm/themes/
    ```

2.  **Set the theme in SDDM configuration:** Edit the SDDM configuration file to set the theme. The configuration file is usually located at `/etc/sddm.conf` or `/etc/sddm.conf.d/default.conf`.  If the file doesn't exist, create it.

    Add or modify the `[Theme]` section to specify the theme name.  The theme name is the same as the directory name you copied in step 1.

    ```
    [Theme]
    Current=archao-sddm
    ```

3.  **Reboot or restart SDDM:**  Reboot your system or restart the SDDM service to apply the changes.

    ```bash
    sudo systemctl restart sddm
    ```

## Configuration

The theme can be configured by editing the `theme.conf` file.  See the comments in that file for details on the available options.

## Dependencies

This theme requires QtQuick and the SddmComponents module.  These should be installed by default on systems using SDDM.

## License

This theme is licensed under the MIT License. See the `LICENSE` file for details.
