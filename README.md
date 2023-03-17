# se-assignment
| Nama | ID Camp |
| --- | --- |
| Amanda Salwa Salsabila | FE4437780 |

## Flowchart
![alt text](https://github.com/amandaslwa/se-assignment/blob/master/Amanda%20Salwa%20Salsabila_FE4437780_Flowchart.png)

## Pseudocode
```
READ AND WRITE barang with string
READ AND WRITE harga barang with number
READ AND WRITE kuantitas barang with number
READ AND WRITE total harga with number
READ AND WRITE uang pembeli with number
READ AND WRITE uang kembalian with number
READ AND WRITE CONDITION terdapat barang di counter kasir with boolean
READ AND WRITE CONDITION terdapat diskon with boolean
READ AND WRITE CONDITION lunas with boolean

PROCEDURE HitungDiskon (harga barang, diskon)
	STORE diskon with diskon divides by 100
	STORE harga barang with harga barang times one minus diskon
END PROCEDURE

PROCEDURE HitungTotalHarga (total harga, harga barang, kuantitas barang)
	STORE total harga with total harga plus harga barang times kuantitas barang
END PROCEDURE

PROCEDURE HitungKembalian (uang pembeli, total harga)
	STORE uang kembalian with uang pembeli minus total harga
END PROCEDURE

PROCEDURE CetakStruk (total harga, uang pembeli, uang kembalian)
	PRINT total harga
	PRINT uang pembeli
	PRINT uang kembalian
END PROCEDURE

SET total harga with 0

WHILE terdapat barang di counter kasir equal 1
DO
	STORE barang with string
	STORE harga barang with number
	STORE kuantitas barang with number
	
	IF terdapat diskon equal 1
		STORE diskon with number
		CALL HitungDiskon(harga barang, diskon)
		CALL HitungTotalHarga(total harga, harga barang, kuantitas barang)
	ELSE IF terdapat diskon equal 0
		CALL HitungTotalHarga(total harga, harga barang, kuantitas barang)
	END IF

	IF terdapat barang di counter kasir equal 0
		EXIT WHILE
	END IF
END WHILE

WHILE lunas equal 0
DO
	STORE uang pembeli with number

	IF uang pembeli more than or equal total harga
		CALL HitungKembalian (uang pembeli, total harga)
		CALL CetakStruk (total harga, uang pembeli, uang kembalian)
	ELSE
		DISPLAY Sorry, your cash is not enough

	IF lunas equal 1
		EXIT WHILE
	END IF
END WHILE
```
