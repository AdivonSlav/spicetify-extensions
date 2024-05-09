name: 🐛 Bug report
description: Report errors or unexpected behavior
labels: [bug]
body:
  - type: checkboxes
    attributes:
      label: 🔍 Is there already an issue for your problem?
      description: Please make sure you are not creating an already submitted <a href="https://github.com/rxri/spicetify-extensions/issues">Issue</a>. Check closed issues as well, because your issue may have already been fixed.
      options:
        - label: I have checked older issues, open and closed
          required: true
  - type: textarea
    attributes:
      label: ℹ Environment / Computer Info
      description: Please provide the details of the system Spicetify is running on.
      value: |
        - Spotify version:
        - Spicetify version:
      placeholder: |
        - Spotify version: Spotify for Windows (64 bit) 1.2.37.701.ge66eb7bc
        - Spicetify version: 2.36.11
      render: Markdown
    validations:
      required: true
  - type: input
    id: extension
    attributes:
      label: 📦 Extension name
      description: Please provide the name of the extension you are having issues with.
      placeholder: ex. adblock
    validations:
      required: true
  - type: textarea
    attributes:
      label: 📝 Description
      description: List steps to reproduce the error and details on what happens and what you expected to happen.
    validations:
      required: true
  - type: textarea
    attributes:
      label: 📸 Screenshots
      description: Place any screenshots of the issue here if possible
    validations:
      required: false