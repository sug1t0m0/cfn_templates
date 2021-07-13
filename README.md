# cfn_templates

##　概要

これは、aws の IAM と Cloud Formation の学習のためのリポジトリである。

## IAMの設計

### IAMユーザグループ(Initial)
- ポリシー
 　- EditableOwnPassword

### IAMユーザグループ(Admin)
- ポリシー
  - AssumeAdministrator
    

### IAMポリシー(EditableOwnPassword)
- 自身のパスワードを変更可能に

### IAMポリシー(AssumeAdministrator)
- アカウント内のIAMユーザであれば, IAMロール(Administrator)にスイッチできる

### IAMロール(Administrator)
- ポリシー
  - AdministratorAccess