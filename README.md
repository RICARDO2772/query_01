# query_01
#CABEÇALHO DA NOTA
SELECT 
	SF2010.F2_CLIENTE, SF2010.F2_EST, SF2010.F2_MENNOTA, SF2010.F2_EMISSAO, SF2010.F2_DOC, SF2010.F2_TRANSP, SF2010.F2_VEICUL1, 
	SF2010.F2_TPFRETE, SF2010.F2_COND

FROM SF2010

WHERE
	SF2010.F2_CLIENTE like '%072189%' AND
	--SD2010.F2_COD LIKE '%MICR-RIC%' AND
	--SF2010.F2_MENNOTA LIKE '%MATELLI%' AND
	SF2010.F2_EMISSAO BETWEEN '20200101' AND '20201109' AND
	SF2010.D_E_L_E_T_ <> '*';
