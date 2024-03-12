# GithubActionsTestQt

QtのプロジェクトをGitHub ActionsでUbuntuとWindows用にビルドしReleaseに実行ファイルをアップロードする例

# 使い方
- ```.github/workflows/release.yaml```をコピペ
- ```env```の```PROJECT_FILE_NAME```, ```DESCTOP_FILE```, ```ICON_FILE```変数をプロジェクトに合わせて設定する
- リポジトリのSettingタブのActions/General/Workflow permissionsを```Read and write permissions```に設定する

# Releaseからダウンロードした実行ファイルの実行方法
## Ubuntu
Releaseから```XXX-Ubuntu-x86_64.AppImage```をダウンロードし以下のコマンドで実行権限を付与してから実行

```
chmod +x XXX-Ubuntu2204-x86_64.AppImage
```

## Windows
Releaseから```XXX-Win-X86_64.zip```をダウンロードし解凍後、中にある```XXX.exe```を実行

初回のみはWindows Defenderによって保護されるため「詳細情報」を押してから「実行」を押して実行する