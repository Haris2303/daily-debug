# 🐞 Daily Debug  

A personal knowledge base for debugging, documenting, and solving errors I encounter in daily development.  
This repo is my "error diary" where I collect problems, solutions, and workarounds – so I (and maybe you) don’t get stuck on the same issue twice.  

---

## 📖 Table of Contents  

1. [Laravel Storage Symlink on Shared Hosting](###laravel-storage-symlink-on-shared-hosting)  
2. More coming soon... 🚀  

---

## 🛠️ Debug Notes  

### 1. Laravel Storage Symlink on Shared Hosting  

On shared hosting, you often can’t run the usual command:  

```bash
php artisan storage:link
```

Instead, create the symlink manually via cPanel or SSH (if enabled):

```bash
ln -s /home/username/laravel/storage/app/public /home/username/public_html/storage
```
