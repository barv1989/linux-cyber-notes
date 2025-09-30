git add lesson4/lesson4_permissions.md
git commit -m "Add lesson4_permissions summary"
git push

cd ~/linux-cyber-notes
mkdir -p lesson4
cat > lesson4/lesson4_permissions.md << 'EOF'
# Linux Permissions Basics (DigitalOcean Summary)

## 1. Пользователи и группы
Linux — многопользовательская ОС: у каждого пользователя есть имя, группа, права.
- Обычные пользователи.
- Системные пользователи.
- Root (суперпользователь) — имеет полный доступ.

## 2. Просмотр прав и владения
Команда:
ls -l
Показывает права доступа, владельца и группу.

Строка формата:
-rw-r--r-- 1 user group size date file.txt
- Первая буква: тип (файл/папка).
- Дальше три блока прав: **owner / group / others**.

## 3. Права (r, w, x)
- `r` (read) — читать файл / просматривать список файлов в папке.
- `w` (write) — изменять файл / создавать или удалять файлы в папке.
- `x` (execute) — запускать файл / заходить в папку.

## 4. Примеры режимов (modes)
rw-  (чтение + запись)
r--  (только чтение)
rwx  (чтение + запись + запуск)

- У каждого файла есть 3 категории: **owner, group, others**.

## 5. Изменение прав и владельца
- `chmod` — меняет права:
chmod 600 file.txt   # только владелец читает и пишет
chmod 755 script.sh  # владелец rwx, остальные r-x

- `chown` — меняет владельца:
sudo chown user file.txt

- `chgrp` — меняет группу:
sudo chgrp developers file.txt

## 6. Числовая и символьная запись
- Числовая:
chmod 640 file.txt
(rw- r-- ---)

- Символьная:
chmod g+r file.txt
(добавить право чтения для группы).

---

## Главное правило безопасности
**Least privilege** — минимально необходимые права.
EOF
