# Endeavour Help
  Repo containing things that help me keep my sanity on Endeavour OS.

## Wi-Fi connection
  View status of network interfaces
  ```bash
  nmcli dev status
  ```

  Check, enable or disable the Wi-Fi radio
  ```bash
  nmcli radio wifi [on/off]
  ```

  List Wi-Fi networks
  ```bash
  nmcli dev wifi list
  ```

  Connect to Wi-Fi network (no password)
  ```bash
  sudo nmcli dev wifi connect "<ssid>"
  ```

  Connect to Wi-Fi network (explicit password)
  ```bash
  sudo nmcli dev wifi connect "<ssid>" password "<password>"
  ```

  Connect to Wi-Fi network (password not shown)
  ```bash
  sudo nmcli --ask dev wifi connect "<ssid>"
  ```
