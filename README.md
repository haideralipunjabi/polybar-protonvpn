# polybar-protonvpn

[ProtonVPN](https://github.com/ProtonVPN/linux-cli) module for [Polybar](https://github.com/jaagr/polybar). Shows the IP Address, Server and Connected Time. Click to Connect / Disconnect

![preview](preview.gif)

## Dependencies

- [protonvpn-cli](https://github.com/ProtonVPN/linux-cli)
- Hack Nerd Font \*

_\* Only if you use the provided icons_

## Usage

Place the given script in some folder, and use it in your polybar `config` as

```
[module/protonvpn]
type = custom/script
exec = "/path/to/script/polybar-protonvpn -o"
tail = true
```

## Customization

You can change the variables in the script to customize some settings

| VARIABLE           | USE                                        |
| ------------------ | ------------------------------------------ |
| COLOR_CONNECTED    | Color of the icon when VPN is connected    |
| COLOR_DISCONNECTED | Color of the icon when VPN is disconnected |
| ICON_CONNECTED     | The icon when VPN is connected             |
| ICON_DISCONNECTED  | The icon when VPN is disconnected          |
| INTERVAL           | Time interval between switching outputs    |
| PRINT_VALUES       | The data to output one by one              |
