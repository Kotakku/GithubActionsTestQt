# GithubActionsTestQt

QtのプロジェクトをGitHub ActionsでUbuntuとWindows用にビルドしReleaseに実行ファイルをアップロードする例

# 使い方
- ```.github/workflows/release.yaml```をコピペ
- ```env```の```PROJECT_FILE_NAME```, ```DESCTOP_FILE```, ```ICON_FILE```変数をプロジェクトに合わせて設定する
- リポジトリのSettingタブのActions/General/Workflow permissionsを```Read and write permissions```に設定する