# Home Assistant – Living Room TV Remote Dashboard

This is an example Lovelace YAML configuration to control a living room TV using Home Assistant and a Broadlink IR blaster.

## 🎯 What It Does

This dashboard lets you control your TV with a clean UI inside Home Assistant. It includes:

- Power on/off  
- Volume up/down (including volume jump buttons like +10 and +50)  
- Channel up/down  
- Input/source switch  
- Mute  
- Directional navigation (Up, Down, Left, Right, OK)  
- Menu, Back, and Android TV Box shortcut  
- Media Player widget integration  

## 🛠 Requirements

- [Home Assistant](https://www.home-assistant.io/)
- A working Broadlink remote integration
- Your TV's IR commands already learned and saved (in this case, the device is called `Samsung2`)
- An entity like `remote.lv_remote` that can send IR commands

## 🧩 How to Use

1. Place the `living_room_tv.yaml` file in your Home Assistant config folder (e.g., under `dashboards/`).
2. In your Home Assistant UI, go to:
   - `Settings` → `Dashboards` → `+ Add Dashboard`
   - Choose "YAML mode" and point it to this file
3. Replace the following with your actual values:
   - `entity_id`: your remote entity (e.g., `remote.lv_remote`)
   - `device_id`: your Broadlink remote device ID
   - `device`: your learned IR profile name (e.g., `Samsung2`)
4. Save and refresh your dashboard.

## 📷 Example Layout

_(Optional: Add a screenshot of the UI layout here to show how it looks.)_

## 💡 Tips

- `num_repeats` is used to send volume commands multiple times (e.g., for +10 or +50)
- `icon_height` helps keep button sizes consistent
- All buttons use `mdi` icons for a modern look

## 🤝 Contributing

Feel free to fork or submit pull requests if you improve this layout or want to add new features like custom macros, additional sources, or dynamic status indicators.

## 📜 License

MIT – Free to use and modify.
