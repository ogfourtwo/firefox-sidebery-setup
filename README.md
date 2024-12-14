# custom firefox-sidebery-setup
My personal clean firefox + sidebery setup which maximizes screenspace without removing anything.

I really loved the look and feel of workspaces and the vertical tabs in Arc Browser but it was very restrictive. As I use a windows device primarily and I like to customize my experiences my go to browser is Firefox. Firefox nightly does have experimental vertical sidebars but it is not a full feature as of yet. I hope they implement a good one soon. This is my setup as of now. I'm very pleased with it.

## Addons used:

1. Sidebery - This addon adds vertical tabs, tab grouping and panels (basically workspaces). 

2. Firefox Color - Lets us customize the firefox theme extensively. 

3. Enable Picture-in-Picture (Optional-Bonus).

Warning: This is a relatively easy process but it does take a few steps and may need tinkering to work properly on your system. This works perfectly as of 12-12-2024 firefox version 133.0 on a 1080p screen. Do this at your own risk.

## Steps:

0. First of all go to settings and enable 'Open previous windows and tabs'.

### Setting Up UserChrome: This is necessary to modify the firefox UI and theme it to your liking. 

1. Open a new tab and go to about:config, click accept and continue. 

2. In the search bar type: toolkit.legacyUserProfileCustomizations.stylesheets and set it to True. 

  ![{A3A556E7-ED41-479D-BCB0-0672C3EDBBDE}](https://github.com/user-attachments/assets/1e73c8e0-d1ad-46c4-9d4b-21949c6056d8)

3. Also set sidebar.verticalTabs to True. This will hide the horizontal tabs and enable firefox's default vertical tabs.

  ![Screenshot 2024-12-14 173917](https://github.com/user-attachments/assets/fdf98fc7-1ab0-4cb2-b119-b7a6379ae061)

4. Click on the pie menu > Help > More Troubleshooting Information

  ![step3](https://github.com/user-attachments/assets/05d21ae7-04d1-4911-b703-7b6687c6314f)

5. Find the 'Profile Folder' row and click on 'Open Folder' (This opens your profile folder)

  ![step4](https://github.com/user-attachments/assets/9fa40f27-29b3-4bfc-bbb5-7091c266539e)

6. In the profile folder create a new folder name it 'chrome'. This is the folder we will be putting our userChrome.css file.

7. Install the [Sidebery addon](https://addons.mozilla.org/en-US/firefox/addon/sidebery/). You must install before going to the next step as the userChrome will hide the default vertical tab bar.

  ![{AF010EE3-9302-44D8-AABA-987AE0CB4EC9}](https://github.com/user-attachments/assets/91388e14-0da2-459e-a8f6-d25f0f75d26d)

9. Create a file userChrome.css and paste the given content or simply download and place the given css file in the 'chrome' folder.

10. Now restart firefox.

### Styling the sidebar

11. In the extensions menu click on the gear icon near sidebery addon and select 'Open Settings'.

  ![{32B25C1E-AF86-465E-A151-CE84D394BC93}](https://github.com/user-attachments/assets/8c71fdbe-ca28-4de3-a66b-c29135f68b9e)

12. In the settings go to 'Help' tab and select 'import addon data' and import the given sidebery.json settings file.

![step12](https://github.com/user-attachments/assets/a2c54740-2d93-48fd-996c-c7cd2e58674c)

13. Now go to 'Styles Editor' tab and paste the content of sidebery-styles.txt into the field.

  ![step13](https://github.com/user-attachments/assets/0e08c57a-3bad-43cd-934c-316134147d08)

### Now we move on to more detailed styling. Feel free to tinker around. 

14. I will now show some of my sidebery settings:
    * enable Use native scroll-bars.
    * enable permissions for the features you want to use.
    * enable Use native context menu.
    * disable Render icons.
      ![{F05979B5-63D9-4E5F-915A-895AD781CE7E}](https://github.com/user-attachments/assets/18bd92ee-b0af-44bc-8392-6b5ffec2a96b)
    * Elements are basically workspaces. You can add them as you like.
      ![step14](https://github.com/user-attachments/assets/c36d13d3-5040-4137-8a46-2a37d401178e)
    * I highly recommend enabling colorized branches.
      ![{2DE6EA42-5AA5-4395-94ED-FD493550FE4F}](https://github.com/user-attachments/assets/59363a93-b6d2-48a0-b7d0-8c6970252684)
    * Snapshots is a feature that remembers windows. It remembers which tabs are open at specific intervals and you can use the snapshots viewer to reopen those tabs. It is a feature that has helped me tons.
      ![{B5CD6CDE-8F64-4E15-9866-EF6AECD7CA58}](https://github.com/user-attachments/assets/17ac225a-cc6b-48f2-8d76-153a2eb4e316)

### Firefox Color (theme)

15. The sidebar does not look good in all themes so I use [Firefox Color addon](https://addons.mozilla.org/en-US/firefox/addon/firefox-color/) to adjust the colors. It is very powerful. I use a full black theme [my theme](https://color.firefox.com/?theme=XQAAAAJWAQAAAAAAAABBqYhm849SCia3ftKEGccwS-xMDPrv2Sw6Caq-qy5QgqeHG4K15QeDoRokmgjiM6AAxM3X9F70ZoGsfXBn8NHNS5chMvkRB4ubMyj96LA5TsM9yBeD-fLr7M3silNCioFfp4gm7DmO058neazgliePszpJuKkqjWpwZpD0bS7e9TSHAUeFjvlgOYd763xF0Jg0x1m5JeeT1ZuXUpZNpFjJqDmjrcC9wOkoxnFXNCZKXYjRRkv5epoER-6YBGybIVHxUW9sQX_-pnAg).

### Toolbar Customization

16. Right click anywhere on the Toolbar (top bar) and click on 'Customize Toolbar'.
    
  ![{4E0F3AC7-E91C-43A7-8B28-352468559156}](https://github.com/user-attachments/assets/8f78d973-6c81-4d1b-8561-00dd9e4821d1)

17. Hide the bookmarks toolbar and also drag it up from under the tool bar.

  ![Screenshot 2024-12-14 183819](https://github.com/user-attachments/assets/9ee7d3a5-2449-4a6b-995a-980cbb4e7245)
  ![step16](https://github.com/user-attachments/assets/eefddeb8-5faf-48eb-99f4-006b292b5d62)

18. You can move any of the icons around. Experiment with it. You can create space between the icons/elements by dragging 'Flexible Space' on there. This is my setup:

  ![{4F22AA0A-41E6-477C-BC3A-39C41FA023AB}](https://github.com/user-attachments/assets/b9c24b1d-94fa-43df-b364-6143d1cf04de)
___
## Credits
* [MrOtherGuy](https://github.com/MrOtherGuy) for his [firefox css hacks](https://github.com/MrOtherGuy/firefox-csshacks)
* [FireFoxCSS](https://www.reddit.com/r/FirefoxCSS/) subreddit for so many resources.
* [akshat46]() for his [FlyingFox](https://github.com/akshat46/FlyingFox/releases) theme that originally inspired me to make my own.
* [FirefoxCSS Store](https://github.com/FirefoxCSS-Store/FirefoxCSS-Store.github.io) for inspiration.
