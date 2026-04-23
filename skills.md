# Навыки и Алгоритмы

## Работа с Git и GitHub

### Настройка безопасного пуша
1. **Получение токена**: Токен должен иметь права `repo` и `workflow`.
2. **Настройка учетных данных**:
   - Использовать `git config --global credential.helper store`.
   - Сохранить токен в файле `~/.git-credentials` в формате: `https://<username>:<token>@github.com`.
   - Не указывать токен напрямую в URL репозитория.
3. **Работа с ветками**:
   - Создавать новые ветки для каждой задачи/изменения.
   - Выполнять коммиты с понятными сообщениями.
   - Отправлять ветку в удаленный репозиторий через `git push -u origin <branch-name>`.

### Пример команды для настройки
```bash
git config --global credential.helper store
echo "https://<username>:<token>@github.com" > ~/.git-credentials
git config --global user.email "<email>"
git config --global user.name "<name>"
```

## Планы
- Добавить навыки работы с GitLab.
- Автоматизация процессов CI/CD.
