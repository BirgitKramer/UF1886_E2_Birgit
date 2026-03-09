# Identificacion flujo
- tabla origen:
```
    sale_order, sale_order_line, res_partner, product_product,product_template
    res_currency
```
- tabla de destino: **sales_clean** 
- tipo de carga: Completa
- Transformacion aplicada:   
- T1 (string operation)
  - Elimina espacios delante y atras(Trim)
  - Campos:
- T2  (replace null)
  - Sustituye campos Null por valores por defecto
  - Evita que valores faltentes rompan al analisis
- T3 (select valores)
  - Convertimos fecha en formato dd-MM-yyyy
  - Forzamos la presición númerica a 16,4 en campos monetarios

