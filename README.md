# LightTheme

### Preparation
1. Make sure that under the **configuration.yaml** file you have the following:

```
frontend:
  themes: !include_dir_merge_named themes
```

2. Under the Home Assistant **Config** folder, create a new folder named **themes**
3. **Restart** Home assistant to apply the changes. 

### HACS installation
1. Go into the Community Store (HACS)
2. Search for **LightTheme**
3. Open the theme
4. Press Install
5. Restart Home Assistant

**If the theme doesn't show up in HACS, you can manually add the repository.**

1. Go into HACS
2. Go to **Frontend**
3. Click on the icon with the 3 dots on the top right
4. Select **Custom Repositories**
5. enter the GitHub URL for the theme under **Repository**
6. Under **Category**, select **Theme**
7. Click on **Add**
8. Search for the theme to add it

### Manual installation
1. In the Home assistant **themes** folder, create a file named `macos_theme.yaml`
2. In this GitHub repo, go into the **themes** folder, open the `macos_theme.yaml` file and copy the content
3. Paste the content in the `macos_theme.yaml` file created under your Home Assistant themes folder

### Enable theme
1. Open your Home Assistant **Profile**
2. Under, **Themes**, select the new **LightTheme**

### Set theme as default for all devices
1. Open **Developer Tools**
2. Go to **Services**
3. Under **Service** enter `frontend.set_theme`
4. Under **Name**, enter `LightTheme`
5. Enable **Mode** and set it to `light`
6. Click on **Call Service**
7. Repeat steps 1 to 6 but change the **Mode** to `dark` 


