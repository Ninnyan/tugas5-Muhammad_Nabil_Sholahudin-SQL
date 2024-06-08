## User Endpoint
|Endpoint|METHOD|BODY|Usage|Example|HEADERS |
|------------|------------|---------|---------|---------|------------|
|/auth/user/register|/POST| "nama": string, "email": string, "password": string,"gender": string,"telephone": string |Register User|-|{Content-Type:: application/json}|
|/auth/user/login|/POST|"email": string, "password": string|Login User|-|-|
|/order/add-order?idWisata={id_wisata}&idUser={id_user}|/POST|"qty"= integer|Order Tiket Wisata|/order/add-order?idWisata=87e458c4b99b4eaaaffb0&idUser=5a4ae7ce110347bd81692|{Authorizations: Bearer {token}, Content-Type: application/json}|
|/order/ordered-tiket?idUser={id_user}|/GET|-|Mendapatkan Riwayat Order Tiket|/order/ordered-tiket?idUser=5a4ae7ce110347bd81692|{Authorizations: Bearer {token}}|
|/order/delete-order?idOrder={id_order}|/DELETE|-|Menghapus Order Tiket|/order/delete-order?idOrder=80e812d61c7143dfad141|{Authorizations: Bearer {token}}|


## Admin Endpoint
|Endpoint|METHOD|BODY|Usage|Example|HEADERS |
|------------|------------|---------|---------|---------|------------|
|/auth-private/admin/register|/POST|"nama": string, "email": string, "password": string,"gender": string,"telephone": string,"admin_key": string,|Register Admin|-|{Content-Type: application/json}|
