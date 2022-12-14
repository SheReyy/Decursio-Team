name: Decursio Project: Expert 1.16.5 - Issue Report
description: Report an issue for our 1.16.5 modpack
labels: [1.16.5, Bug, Unreviewed]
body:    
  - type: markdown
    attributes:
      value: "## Versions"
  
  - type: input
    id: modpack-version
    attributes:
      label: Modpack Version
      placeholder: "Ex: Beta 22"
      description: "'Latest' is not a valid answer, write an exact version number"
    validations:
      required: true
  - type: input
    id: launcher-used
    attributes:
      label: Launcher Used
      placeholder: "Ex: Curseforge, MultiMC"
    validations:
      required: true
  - type: dropdown
    id: optifine-presence
    attributes:
      label: Do you, or did you had Optifine installed when the issue took place?
      options:
        - 'Yes'
        - 'No'
    validations:
      required: true
   - type: dropdown
    id: just-tinkers
    attributes:
      label: "Tried reproducing without Optifine?"
      options:
        - 'Yes'
        - 'I will go do that now'
        - 'No'
    validations:
      required: true
\
  
  
  - type: markdown
    attributes:
      value: "## Issue Description"

  - type: textarea
    id: description
    attributes:
      label: Describe your issue
    validations:
      required: true
      
   - type: input
   id: log-file
   attributes:
     label: Log File related to your crash
     description: Paste a link to the log file
   validations:
     required: true
  
  - type: input
    id: crash-report
    attributes:
      label: Crash Report
      description: Paste a link to the crash report, if present
    validations:
      required: false
      
  - type: textarea
    id: other-mods
    attributes:
      label: Other mods
      description: List the additional mods used while the issue took place
    validations:
      required: true
        
        
  - type: markdown
    attributes:
      value: "## Confirm the following"
  
      
  - type: dropdown
    id: searched
    attributes:
      label: "Searched for known issues?"
      description: "Select all that apply. Please check the [known-issue](https://discord.com/channels/879788820265074698/892054075145863179) and the [faq](https://discord.com/channels/879788820265074698/912742834212327445) channels on our discord server."
      multiple: true
      options:
        - 'Checked know-issues'
        - 'Checked faq'
        - 'Searched open issues'
        - 'Searched closed issues'
        - 'I did not search'
    validations:
      required: true