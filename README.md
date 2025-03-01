# Flutter Meetup Berlin Workshop

## Getting Started

1. Fork this repository.
1. **[IMPORTANT]** **Enable actions** by going to `Actions` -> `I understand my workflows, go ahead and enable them`.
1. Clone the forked repository.

   ```bash
   git clone https://github.com/<your-username>/flutter-meetup-berlin.git
   ```

1. Open the project in VSCode.

   ```bash
   code flutter-meetup-berlin
   ```

1. Bootstrap App

   ```bash
   flutter pub get    # Install deps
   flutter gen-l10n   # Generate localization files
   ```

1. Bootstrap Widgetbook

   ```bash
   cd widgetbook/
   flutter pub get                 # Install deps
   dart run build_runner watch -d  # Watch for generator changes
   ```

1. Run Widgetbook from VSCode (to enable hot reload)

## Widgetbook Challenge

1. Add the missing `PrimaryButton` [use-case](./widgetbook/lib//ui/widgets/primary_button.dart).

## Widgetbook Cloud Challenge

1. Sign up to [Widgetbook Cloud](https://app.widgetbook.io).
1. Create a new **workspace**.
1. Create a new project by **importing** your forked repository.
1. Get the **API key** from the **project's settings**.
1. Add the **API key** to your **repository's secrets** as `WIDGETBOOK_CLOUD_API_KEY` by going to `Settings` -> `Secrets and Variables` -> `Actions` -> `New repository secret`.
1. Commit the new use-case to the repository's `main` branch.

   ```bash
   git add .
   git commit -m "feat(widgetbook): add button use-case"
   git push -u origin main
   ```

1. Fix the **button radius**, to match the [design](https://www.figma.com/design/HsANkdhbsCNTkXBzNJRNLD/Groceries-Demo?node-id=7235-4663&t=N6qwmLP7MP59ClWB-4).
1. **Commit** your changes on a **new branch**.

   ```bash
   git checkout -b fix/increase-button-radius
   git add .
   git commit -m "fix: increase button radius"
   git push -u origin fix/increase-button-radius
   ```

1. Create a new **pull request**.
1. Wait for CI to finish, then check the **Widgetbook Cloud status checks**.

## Resources

- [🔗 Figma File](https://www.figma.com/design/HsANkdhbsCNTkXBzNJRNLD/Groceries-Demo?node-id=7225-2991&t=4oLAnrUYEax8YzGo-1)
- [🔗 Widgetbook Docs](https://docs.widgetbook.io/)
- [🔗 Widgetbook Cloud](https://app.widgetbook.io)
