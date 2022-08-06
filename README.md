# Swift Lint

SwiftLint: https://github.com/realm/SwiftLint

## Downloads

1. Homebrew: https://brew.sh

2. `swiftlint`: https://formulae.brew.sh/formula/swiftlint using `brew install swiftlint`

## Project Configuration

Add this to your project under **Project - Build Phases - Create new Run Script **

<img width="818" alt="Screen Shot 2022-08-05 at 9 27 57 PM" src="https://user-images.githubusercontent.com/75696759/183228221-5f192951-02ff-4d19-a1f9-62b7a87c0152.png">

```txt
export PATH="$PATH:/opt/homebrew/bin"
if which swiftlint > /dev/null; then
  swiftlint
else
  echo "warning: SwiftLint not installed, download from https://github.com/realm/SwiftLint"
fi
```

## Autocorrect

Command: `swiftlint autocorrect`

Make sure you review what the autocorrect tool did using `git diff`
