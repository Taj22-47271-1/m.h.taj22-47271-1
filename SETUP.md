# GitHub Profile Setup Guide for M.H. Taj

This package is prepared for the GitHub account:

```text
Taj22-47271-1
```

## 1. Create the profile repository

Create a new **public** repository with this exact name:

```text
Taj22-47271-1
```

GitHub profile READMEs work only when the repository name matches the username.

## 2. Upload the package

Upload these items to the repository root:

```text
README.md
assets/
.github/
```

Do not upload the ZIP file itself. Extract it first.

## 3. Commit the files

Use a commit message such as:

```text
Create professional GitHub profile README
```

## 4. Enable GitHub Actions write permission

Open:

```text
Repository → Settings → Actions → General
```

Under **Workflow permissions**, select:

```text
Read and write permissions
```

Then click **Save**.

## 5. Generate the 3D graph

Open:

```text
Actions → GitHub-Profile-3D-Contrib → Run workflow
```

Wait for the workflow to finish successfully.

It will create:

```text
profile-3d-contrib/
```

## 6. Generate the contribution snake

Open:

```text
Actions → Generate Contribution Snake → Run workflow
```

Wait for the workflow to finish successfully.

It will create:

```text
dist/
```

## 7. Refresh the profile

Open:

```text
https://github.com/Taj22-47271-1
```

The banner, profile information, skills, projects, certificates, statistics, 3D graph, and contribution snake should appear.

## Optional: Add a CV button

Upload your CV to the repository root using this filename:

```text
cv.pdf
```

Then place this code near the social buttons in `README.md`:

```html
<a href="./cv.pdf">
  <img src="https://img.shields.io/badge/CV-Download-7C4DFF?style=for-the-badge&logo=readthedocs&logoColor=white" alt="Download CV" />
</a>
```

## Updating later

After editing files locally:

```bash
git add .
git commit -m "Update profile README"
git push origin main
```

## Troubleshooting

### README does not appear

Confirm that:

- Repository name is exactly `Taj22-47271-1`
- Repository is public
- `README.md` is in the root folder
- `README.md` is not empty

### Workflow cannot push

Enable:

```text
Settings → Actions → General → Workflow permissions → Read and write permissions
```

### 3D graph or snake is blank

Run each workflow manually once from the **Actions** tab, then wait for the generated files to be committed.
