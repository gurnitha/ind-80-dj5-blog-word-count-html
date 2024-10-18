# ind-80-dj5-blog-word-count-htmx
Membuat aplikasi blog menggunakan Django versi 5.x dan HTMX

## 1. SETUP

#### 1. Lokasi

#### 2. Membuat remote repositori

#### 3. Mengklon remote repositori

#### 4. Membuat lingkungan virtual

#### 5. Menginstal Django


## 2. PROYEK DJANGO

#### 1. Membuat proyek Django

        modified:   README.md
        new file:   config/config/__init__.py
        new file:   config/config/asgi.py
        new file:   config/config/settings.py
        new file:   config/config/urls.py
        new file:   config/config/wsgi.py
        new file:   config/manage.py

#### 2. Membuat root direktori 'src'

        modified:   README.md
        renamed:    config/config/__init__.py -> config/__init__.py
        renamed:    config/config/asgi.py -> config/asgi.py
        renamed:    config/config/settings.py -> config/settings.py
        renamed:    config/config/urls.py -> config/urls.py
        renamed:    config/config/wsgi.py -> config/wsgi.py
        renamed:    config/manage.py -> manage.py

#### 3. Menjalankan server Django

#### 4. Mejalankan migrasi untuk mengakses admin panel

#### 5. Membuat superuser


## 3. SETTINGS

#### 1. Menseting bahasa dan waktu

        modified:   README.md
        modified:   config/settings.py

#### 2. Menseting absolute path untuk templates

        modified:   README.md
        modified:   config/settings.py

        # testing
        (venv312511) λ python manage.py check

        # results
        C:\Users\ING\Desktop\workspace\80-ind-dj5-jadual-vaksin\src\config\settings.py
        C:\Users\ING\Desktop\workspace\80-ind-dj5-jadual-vaksin\src\config
        C:\Users\ING\Desktop\workspace\80-ind-dj5-jadual-vaksin\src

        System check identified no issues (0 silenced).

#### 3. Menseting absolute path untuk file statis

        modified:   README.md
        modified:   config/settings.py

        (venv312511) λ python manage.py check
        System check identified no issues (0 silenced).

#### 4. Menseting absolute path untuk file media

        modified:   README.md
        modified:   config/settings.py
        modified:   config/urls.py

        (venv312511) λ python manage.py check
        System check identified no issues (0 silenced).


## 4. DATABASE

#### 1. Membuat postgres database

        E:\_WORKSPACE\laragon\www
        λ psql -U postgres
        psql (16.2)
        WARNING: Console code page (437) differs from Windows code page (1252)
                 8-bit characters might not work correctly. See psql reference
                 page "Notes for Windows users" for details.
        Type "help" for help.

        postgres=# CREATE DATABASE ind_80_dj5_blog_word_count_htmx;
        CREATE DATABASE
        postgres=#

#### 2. Menseting path untuk menghubungan proyek ke database

        # DB: PostgreSQL
        DATABASES = {
            'default': {
                'ENGINE': 'django.db.backends.postgresql_psycopg2',
                'NAME': 'ind_80_dj5_blog_word_count_htmx', 
                'USER': 'postgres', 
                'PASSWORD': 'postgres',
                'HOST': 'localhost', 
                'PORT': '5433',
            }
        }

          File "C:\Users\ING\Desktop\workspace\ind-80-dj5-blog-word-count-htmx\venv312511\Lib\site-packages\django\db\backends\postgresql\base.py", line 29, in <module>
            raise ImproperlyConfigured("Error loading psycopg2 or psycopg module")
        django.core.exceptions.ImproperlyConfigured: Error loading psycopg2 or psycopg module

        modified:   README.md
        modified:   config/settings.py