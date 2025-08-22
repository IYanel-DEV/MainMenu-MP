# 🎮 Godot Multi-Theme Main Menu Collection

A collection of beautiful, fully customizable main menu themes for Godot Engine with seamless theme switching functionality.

## ✨ Features

- **4 Distinct Themes**: Dark, Purple, Red, and Light themes
- **Real-time Theme Switching**: Switch between themes instantly with a single button
- **Complete UI Elements**: 
  - Main menu buttons (Host Game, Join Game, Server Browser, Settings, Quit)
  - Player information panel with name input
  - Network information display
  - Connection status indicator
  - Version information
- **Polished Design**: Custom StyleBox resources with rounded corners, shadows, and smooth transitions
- **Ready to Use**: Drop into any Godot project and customize as needed

## 🎨 Theme Showcase
Click on each section to view the screenshots:

<details>
<summary>Purple</summary>
<br>
<img width="1153" height="649" alt="Plugin Interface 1" src="https://github.com/user-attachments/assets/eefe7e29-beb7-4ae2-982e-5c27151be8c8">
</details>

<details>
<summary>Black</summary>
<br>
<img width="1153" height="649" alt="Plugin Interface 2" src="https://github.com/user-attachments/assets/aa3643bc-16f1-48f4-b07e-daaa6957bb86">
</details>

<details>
<summary>Red</summary>
<br>
<img width="1153" height="649" alt="Plugin Interface 3" src="https://github.com/user-attachments/assets/3c6d0a5c-9c67-439a-b688-eaa3067a03ef">
</details>

<details>
<summary>White</summary>
<br>
<img width="1153" height="649" alt="Plugin Interface 4" src="https://github.com/user-attachments/assets/c395cbb2-1402-45bf-a201-673fb55ece9f">
</details>

### 🌙 Dark Theme
- **Background**: Deep dark blue-gray (`Color(0.05, 0.05, 0.08, 1)`)
- **UI Elements**: Sleek black buttons with gray borders
- **Perfect for**: Modern, professional game interfaces

### 💜 Purple Theme  
- **Background**: Rich purple gradient (`Color(0.1, 0.05, 0.2, 1)`)
- **UI Elements**: Purple-themed buttons and panels
- **Perfect for**: Fantasy, magical, or creative games

### 🔴 Red Theme
- **Background**: Deep crimson (`Color(0.08, 0.02, 0.02, 1)`)
- **UI Elements**: Bold red styling with warm tones
- **Perfect for**: Action, horror, or intense gameplay experiences

### ☀️ Light Theme
- **Background**: Clean light blue-white (`Color(0.96, 0.97, 0.99, 1)`)
- **UI Elements**: Bright, modern design with subtle shadows
- **Perfect for**: Casual, family-friendly, or minimalist games

## 🚀 Quick Start

1. **Download** the scene files from this repository
2. **Import** into your Godot project
3. **Add** the main menu scene to your project
4. **Customize** colors, text, and functionality as needed

## 📁 Project Structure

```
MainMenuThemes/
├── MainMenu_Dark.tscn      # Dark theme variant
├── MainMenu_Purple.tscn    # Purple theme variant  
├── MainMenu_Red.tscn       # Red theme variant
├── MainMenu_Light.tscn     # Light theme variant
└── README.md              # This file
```

## 🛠️ Customization

### Changing Colors
Each theme uses `StyleBoxFlat` resources that can be easily modified:
- **Button Colors**: Modify `bg_color` and `border_color` properties
- **Panel Styling**: Adjust transparency and corner radius
- **Font Colors**: Update `theme_override_colors/font_color`

### Adding Functionality
Connect button signals in your script:
```gdscript
func _ready():
    $UI/MainContainer/MenuButtons/HostGameBtn.pressed.connect(_on_host_game)
    $UI/MainContainer/MenuButtons/JoinGameBtn.pressed.connect(_on_join_game)
    # Add more connections as needed

func _on_host_game():
    # Your host game logic here
    pass
```

### Theme Switching
The theme toggle button allows runtime switching between different visual styles. Implement your switching logic:
```gdscript
func _on_theme_toggle():
    # Switch between theme scenes or modify StyleBox resources
    pass
```

## 🎯 UI Components

### Main Menu Buttons
- **Host Game**: Start a multiplayer server
- **Join Game**: Connect to existing server  
- **Server Browser**: Browse available servers
- **Settings**: Game configuration options
- **Quit**: Exit the application

### Information Panels
- **Player Info**: Name input and status display
- **Network Info**: IP address, port, and player count
- **Version Label**: Game version and credits

## 🔧 Technical Details

- **Godot Version**: Compatible with Godot 4.x
- **Scene Format**: `.tscn` files with embedded resources
- **Styling**: Custom `StyleBoxFlat` resources
- **Layout**: Responsive anchor-based positioning
- **Performance**: Optimized with minimal draw calls

## 🤝 Contributing

Feel free to:
- Submit bug reports
- Suggest new themes or features
- Create pull requests with improvements
- Share screenshots of your customizations

## 📝 License

This project is open source. Feel free to use, modify, and distribute in your own projects.

## 🙏 Credits

**Created by**: Yanel  
**Engine**: Godot Engine  
**Version**: v1.0.0

---

### 💡 Pro Tips

- Use the theme toggle to test different moods for your game
- Combine elements from different themes to create your unique style  
- The modular design makes it easy to add new themes
- All themes maintain consistent functionality across visual variants

**⭐ If this helped your project, consider giving it a star!**
