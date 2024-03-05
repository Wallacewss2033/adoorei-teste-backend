## Instalação 


- Clone o projeto
```
git clone git@github.com:Wallacewss2033/adoorei-teste-backend.git
```
- Entre na pasta do prejeto e clone este
```
git clone git@github.com:Wallacewss2033/ecommerce-abc.git
```

### Back-end

- Entre na pasta do projeto ecommerce-abc e instale as dependencias
```
composer install
```
- logo após rode esses comandos
```
cp .env.example .env
```
```
php artisan key:generate
```

- Não esqueça de configurar o banco de dados na ``` .env ```
  
![image](https://github.com/Wallacewss2033/fullstack-challenge-20231205/assets/39920409/ec726dce-7762-4c68-b66c-668698afad41)

- Na pasta raíz do projeto deixe
```
docker-compose up -d --build
```

-entre no terminal do projeto ``` ecommerce-abc ``` e Para criar o banco de dados
```
php artisan migrate
```

- Para popular o banco na tabela de produtos
```
php artisan db:seed
```

OBS: CASO HAJA ALGUM PROBLEMA DE PERMISSÃO NO PROJETO RODE:

- chown -R root:www-data storage
- chmod -R 777 ./storage
- chmod -R 775 ./storage
