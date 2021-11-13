# Aplikasi Invoice Management #

Aplikasi ini dipakai untuk mengelola invoice dan menyambungkan dengan berbagai metode pembayaran
Diantar metode pembayaran yang akan disupport antara lain :

* Virtual Account Bank
  * Bank BNI
  * Bank CIMB
  * Bank BSI

* e-Wallet
  * Ovo
  * GoPay

* QR Payment
  * QRIS



# Cara Setup Database #

1. Jalankan postgresql di docker

```
docker run --rm \
--name spring-invoice \
-e POSTGRES_DB=springinvoicedb2 \
-e POSTGRES_USER=springinvoice \
-e POSTGRES_PASSWORD=springinvoice123 \
-e PGDATA=/var/lib/postgresql/data/pgdata \
-p 5432:5432 \
postgres
```


# CARA MASUK KE POSTGRESQL #

```
psql -h localhost -p 5444 -U springinvoice springinvoicedb
```