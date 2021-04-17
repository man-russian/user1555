# github email, SSH и GPG
Чтобы держать мои адреса электронной почты в секрете откройте Settings/Emails установите галочку
 -[x] Keep my email addresses private (по умолчанию уже включено)
В комментарии к этой карточке указан адрес почты в формате 19236790+user@users.noreply.github.com его желательно использовать в git config user.email и в gpg ключах.
Чтобы подписывать все коммиты по умолчанию в любом локальном репозитории на вашем компьютере, запустите.
```bash
git config --global commit.gpgsign true
```

```bash
git config user.signingKey <keyID>
```
```bash
git log --show-signature
```

Чтобы подписать тег, добавьте `-s` в команду `git tag`.
```bash
git tag -s mytag
# Создает подписанный тег
```
Проверьте свой подписанный тег, запустив `git tag -v [tag-name]`.
```bash
git tag -v mytag
# Проверяет подписанный тег
```

