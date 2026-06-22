# GitHub Setup Checklist

Follow these steps to fully activate your new GitHub profile!

## 1. Enable GitHub Actions
- Navigate to your repository (`PrajitPranav/PrajitPranav`).
- Click on the **Settings** tab.
- In the left sidebar, expand the **Actions** section and click on **General**.
- Under **Actions permissions**, select **Allow all actions and reusable workflows**.
- Click **Save**.

## 2. Enable Read and Write Workflow Permissions
- Still in **Settings** > **Actions** > **General**.
- Scroll down to the **Workflow permissions** section.
- Select **Read and write permissions**.
- Check the box for **Allow GitHub Actions to create and approve pull requests** (optional, but good practice for other actions).
- Click **Save**.

## 3. Manually Run Generate Snake Workflow
- Click on the **Actions** tab at the top of your repository.
- On the left sidebar, click on **Generate Snake**.
- Click the **Run workflow** dropdown button on the right side.
- Leave the branch as `main` and click **Run workflow**.
- Wait for the job to complete (it should take a minute or two and turn green).

## 4. Verify Output Branch Creation
- Go to the **Code** tab of your repository.
- Click the branch dropdown (usually says `main`).
- Verify that a new branch named `output` has been created.
- You can switch to the `output` branch to verify the `github-contribution-grid-snake.svg` and `github-contribution-grid-snake-dark.svg` files exist.

## 5. Common Fixes if Snake Animation Doesn't Appear
- **Broken Image Link**: Make sure the branch name in your README matches the actual branch name (e.g., `output`).
- **Permissions Issue**: Double check that your Workflow Permissions are set to **Read and write permissions** (Step 2).
- **Workflow Failed**: Go to the **Actions** tab and click on the failed run. Check the logs to see what error occurred. Often, this happens if `GITHUB_TOKEN` lacks permissions.
- **Cache Delay**: Sometimes GitHub caches images for a few minutes. Try hard-refreshing your browser (`Ctrl+F5` or `Cmd+Shift+R`).
