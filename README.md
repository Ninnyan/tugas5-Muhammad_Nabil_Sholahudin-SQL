# User Flow
| Endpoint|METHOD|BODY|Usage|Example|HEADERS |
|------------|------------|---------|---------|---------|------------|
|/auth/user/register|/POST| "nama": string, "email": string, "password": string,"gender": string,"telephone": string | POST Registrasi|-|{Content-Type}|
|/auth/user/login|/POST|"email": string, "password": string|POST Login|-|-|
|/order/add-order?idWisata={id_wisata}&idUser={id_user}|/POST|"qty"= integer|POST Order|/order/add-order?idWisata=87e458c4b99b4eaaaffb0&idUser=5a4ae7ce110347bd81692|{Authorizations: Bearer {token}, Content-Type: application/json}|
