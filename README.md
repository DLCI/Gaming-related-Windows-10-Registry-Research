# Gaming-related-Windows-10-Registry-Research

There is a great deal of mis-information present on the internet regarding "tweaks" which supposedly offer some kind of benefit for competitive minded gamers.
Most users who post such "tweaks" do not actually understand what these tweaks do or how they work.

Many of these so-called "gaming tweaks" can actually introduce detrimental inconsistencies or alter windows behavior in a way that will result in mild performance loss, rather than improvements.

I have spent the last several years digging through the Windows 10 registry and using an evidence based approach (wherever possible) to determine what changes to default settings will actually provide a consistent and verifiable benefit to gaming-minded users.

While I have spent a considerable amount of time and energy verifying that the same behavior results from the same change to a default setup by completely re-installing windows and making the same changes in the same sequence dozens of times, I will caution that despite this, I cannot guarantee that your results will be identical.

Thus, all information is provided "as-is" and I cannot take responsibility for anything unexpected that results from your use of this information.  Please do not contact me about issues that result from any changes you make to your own settings, as I will be unable to assist you.



CHANGES YOU MAKE TO YOUR OWN REGISTRY SHOULD ONLY BE MADE AFTER SAVING A BACKUP OF YOUR EXISTING SETTINGS AND SHOULD BE DONE AS CAREFULLY/CONSERVATIVELY AS POSSIBLE. 


Finally, some of these key-changes were discovered as part of my own attempts to resolve minor issues with my system, and thus they may not be relevant for everyone.  These will be clearly marked as such along with a description of the specific circumstances under which they are relevant.

It is highly recommended that you do not make any changes to the registry that are not relevant to your own setup.

WIP draft of planned research sections

Current sub-sections

    Desktop and Desktop DPI-related information
      Includes 
       Desktop-settings registry keys that are read on startup
            * which keys should exist by default
                >> A repository of all the default values for every registry sub-section mentioned on this page will eventually be added
                >> The intent is to provide a comprehensive resource for users who have made changes to their own settings that they now wish to undo.
        Desktop-settings which are read on startup but are not present by default
            * which keys should be added to the default settings
        Desktop-Settings read on startup which are present under multiple different built-in user accounts
            * which keys should be modified in multiple locations to ensure consistent behavior

    DWM related information 
      Includes
       An explanation on how the DWM rendered desktop may disrupt mouse-input behavior and why this is relevant for fullscreen applications
        DWM registry keys that are read on startup
            * which keys should exist by default
            * which keys are read on startup but do not exist by default
        DWM related registry changes with a demonstrable effect that I have been unable to verify is beneficial
            * how to force the DWM rendered virtual desktop overlay (which is hidden but remains active) to operate identically to the active fullscreen application
                >> this section contains ongoing research and may include behavior altering changes that I have yet to empirically verify is an improvement over default
      
    Multi-monitor related Information
       Includes
        An explanation on how/why multi-monitor setups can alter mouse-input behavior
        What setupts are likely to be affected by this
        DWM related registry keys

    Power-setting related information
        Includes
          An explanation of how power-policy works by default and how it is organized
          An explanation on why it is beneficial to expose certain hidden settings
          A list of keys related to settings with a beneficial effect but are not visible in the settings menu
             * USB power settings
             * idle timers/timeouts
             * Other
       

    Misc Non-present registry Keys read upon boot that may be relevant
       Includes
         Fullscreen enhanced settings under gameconfigstore
          Keyboard settings
         Touchpad/pen input settings
      

    Other non-registry changes
       Includes
          Group policy edits
             GDI scaling policy changes
               * A list of applications that GDI policy changes should be applied to, with verified improvement 
               * A comprehensive list of all processes that GDI policy changes affect that I have not empirically verified results in improvement
              Power Policy changes
               * Throttling changes
               * How to force specific power schemes hidden from the settings menu

      Assigning interrupts
            * Why this may improve your system
            * What kind of a system may benefit from assigning interrupts
            * General guidelines on how to design an interrupt scheme for your own system
              >> The two methods of assigning interrupts
                  // Option A: Assigning single processor interrupts to IRQ registered devices
                  // Option B: Assinging a MSI distributed interrupt scheme
                  
                  
