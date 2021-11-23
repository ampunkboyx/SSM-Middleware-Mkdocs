# DATA MAPPING ROB
## BUSINESS PROFILE
	Service	getBizProfile
PDF TEMPLATE	
## Page 1	
<style type="text/css">
	table.tableizer-table {
		font-size: 12px;
		border: 1px solid #CCC; 
		font-family: Arial, Helvetica, sans-serif;
	} 
	.tableizer-table td {
		padding: 4px;
		margin: 3px;
		border: 1px solid #CCC;
	}
	.tableizer-table th {
		background-color: #104E8B; 
		color: #FFF;
		font-weight: bold;
	}
</style>
<table class="tableizer-table">
<thead><tr class="tableizer-firstrow"><th>TITLE :</th><th>Business information (ENG)</th><th clos>Maklumat Perniagaan(Malay)</th><th>&nbsp;</th><th>&nbsp;</th><th>Page 1</th><th>&nbsp;</th></tr></thead><tbody>
 <tr><td>Column Name(English)</td><td>Column Name(MALAY)</td><td>&nbsp;</td><td>Remarks</td><td>json Node / Middleware</td><td>Object Name</td><td>&nbsp;</td></tr>
 <tr><td>Business Name</td><td>NAMA PERNIAGAAN</td><td>&nbsp;</td><td>&nbsp;</td><td>registrationName</td><td>robBusinessInfo</td><td>&nbsp;</td></tr>
 <tr><td>Business Registrations No</td><td>NO.PENDAFTARAN PERNIAGAAN</td><td>&nbsp;</td><td>200803090077<br>(SA0085324-V)</td><td>registrationNo<br>checkDigit</td><td>robBusinessInfo</td><td>&nbsp;</td></tr>
 <tr><td>12-digit new ?</td><td>&nbsp;</td><td>&nbsp;</td><td>200803090077</td><td>newFormatNo</td><td>GetNewFormatEntity</td><td>&nbsp;</td></tr>
 <tr><td>Company No.</td><td>&nbsp;</td><td>&nbsp;</td><td>SA0085324</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td></tr>
 <tr><td>Check Digit</td><td>&nbsp;</td><td>&nbsp;</td><td>V</td><td>&nbsp;</td><td>&nbsp;</td></tr>
 <tr><td>Principle Place of Business</td><td>ALAMAT UTAMA PERNIAGAAN</td><td>&nbsp;</td><td>&nbsp;</td><td>mainAddress1</td><td>robBusinessInfo</td><td>&nbsp;</td></tr>
 <tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>mainTown</td><td>robBusinessInfo</td><td>&nbsp;</td></tr>
 <tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>mainPostcode</td><td>robBusinessInfo</td><td>&nbsp;</td></tr>
 <tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>mainState</td><td>robBusinessInfo</td><td>&nbsp;</td></tr>
 <tr><td>Business OwnerShip</td><td>BENTUK PERNIAGAAN</td><td>&nbsp;</td><td><b>Malay</b><br> Jika =1, PEMILIKAN TUNGGAL. <br> Jika > 1, PERKONGSIAN <br> <b>English</b> <br> if = 1, SOLE PROPRIETORSHIP <br> if >1 PARTNERSHIP</td><td>ownerCount</td><td>robBusinessInfo</td><td>&nbsp;</td></tr>
 <tr><td>Business Start Date</td><td>TARIKH MULA BERNIAGA</td><td>&nbsp;</td><td>&nbsp;</td><td>startBusinessDate</td><td>robBusinessInfo</td><td>&nbsp;</td></tr>
 <tr><td>Registration Date</td><td>TARIKH PENDAFTARAN</td><td>&nbsp;</td><td>&nbsp;</td><td>registrationDate</td><td>robBusinessInfo</td><td>&nbsp;</td></tr>
 <tr><td>Business Expiry Date</td><td>TARIKH LUPUT PENDAFTARAN</td><td>&nbsp;</td><td>&nbsp;</td><td>endBusinessDate</td><td>robBusinessInfo</td><td>&nbsp;</td></tr>
 <tr><td>LAST AMMENDMEND DATE</td><td>TARIKH PERUBAHAN TERAKHIR</td><td>&nbsp;</td><td>* need to view this column if value exist</td><td>ammendmentDate</td><td>robBusinessInfo</td><td>&nbsp;</td></tr>
 <tr><td>STATUS</td><td>STATUS</td><td>&nbsp;</td><td><b>A</b>-active,<br> <b>L</b>-Expired,<br> <b>T</b>-Terminated,<br> <b>B</b>-LLP Conversion</td><td>status</td><td>robBusinessInfo</td><td>Aktif, Luput, Penamatan, Bubar-Pertukaran kepada Perkongsian Liabiliti Terhad (PLT)</td></tr>
 <tr><td>TERMINATION DATE</td><td>TARIKH PENAMATAN</td><td>&nbsp;</td><td>* need this to view if STATUS=Terminated</td><td>terminationDate</td><td>robBusinessInfo</td><td>* Tiada Dalam Sijil</td></tr>
 <tr><td>LLP NAME</td><td>NAMA PLT</td><td>&nbsp;</td><td>* need to view if status is B- Conversion to LLP</td><td>llpName</td><td>robBusinessInfo</td><td>* Tiada Dalam Sijil</td></tr>
 <tr><td>LLP NUMBER</td><td>NOMBOR PLT</td><td>&nbsp;</td><td>* need to view if status is B- Conversion to LLP</td><td>llpNo</td><td>robBusinessInfo</td><td>* Tiada Dalam Sijil</td></tr>
 <tr><td>CONVERSION DATE</td><td>TARIKH PERTUKARAN</td><td>&nbsp;</td><td>* need to view if status is B- Conversion to LLP</td><td>llpconvertDate</td><td>robBusinessInfo</td><td>* Tiada Dalam Sijil</td></tr>
</tbody></table>

<table class="tableizer-table">
<thead><tr class="tableizer-firstrow"><th>TITLE :</th><th>Business Type (eng)</th><th>JENIS PERNIAGAAN(MALAY)</th><th>&nbsp;</th><th>&nbsp;</th><th>&nbsp;</th></tr></thead><tbody>
 <tr><td>Column Name(English)</td><td>Column Name(MALAY)</td><td>&nbsp;</td><td>Remarks</td><td>json Node</td><td>Object Name</td></tr>
 <tr><td>Business Type</td><td>JENIS PERNIAGAAN</td><td>&nbsp;</td><td>&nbsp;</td><td>description</td><td>robBusinessInfo</td></tr>
</tbody></table>

<table class="tableizer-table">
<thead><tr class="tableizer-firstrow"><th>TITLE:</th><th>Branch information(eng)</th><th>MAKLUMAT CAWANGAN(MALAY)</th><th>&nbsp;</th><th>&nbsp;</th><th>&nbsp;</th></tr></thead><tbody>
 <tr><td>Column Name(English)</td><td>Column Name(MALAY)</td><td>&nbsp;</td><td>Remarks</td><td>json Node</td><td>Object Name</td></tr>
 <tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>No Column name. base on pdf design just List the branch address accordingly. </td><td>address1</td><td>robBranchListInfo</td></tr>
 <tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>town</td><td>robBranchListInfo</td></tr>
 <tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>postcode</td><td>robBranchListInfo</td></tr>
 <tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>state</td><td>robBranchListInfo</td></tr>
 <tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>status</td><td>robBranchListInfo</td></tr>
</tbody></table>

## Page 2
<table class="tableizer-table">
<thead><tr class="tableizer-firstrow"><th>TITLE:</th><th>Information of current owner(eng)</th><th>MAKLUMAT PEMILIK PERNIAGAAN TERKINI(MALAY)</th><th>&nbsp;</th><th>Page:</th><th>2</th></tr></thead><tbody>
 <tr><td>Column Name(English)</td><td>Column Name(MALAY)</td><td>&nbsp;</td><td>Remarks</td><td>json Node</td><td>Object Name</td></tr>
 <tr><td>Business Name</td><td>NAMA PERNIAGAAN</td><td>&nbsp;</td><td>&nbsp;</td><td>registrationName</td><td>robBusinessInfo</td></tr>
 <tr><td>Business Registrations No</td><td>NO.PENDAFTARAN PERNIAGAAN</td><td>&nbsp;</td><td>200803090077 (SA0085324-V)</td><td>registrationNo<br>checkDigit</td><td>robBusinessInfo</td></tr>
 <tr><td>12-digit new</td><td>12 Digit Baru</td><td>&nbsp;</td><td>200803090077</td><td>NewFormatNo</td><td>GetNewFormatEntityno</td></tr>
 <tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>SA0085324</td><td>&nbsp;</td><td>&nbsp;</td></tr>
 <tr><td>Check Digit</td><td>&nbsp;</td><td>&nbsp;</td><td>V</td><td>&nbsp;</td><td>&nbsp;</td></tr>
 <tr><td>Name</td><td>NAMA</td><td>&nbsp;</td><td>This object took from list of robOwnershipListInfo with status = A . It means for current owner</td><td>ownerName</td><td>robOwnerShipInfos</td></tr>
 <tr><td>Residential Address</td><td>ALAMAT KEDIAMAN</td><td>&nbsp;</td><td>&nbsp;</td><td>address1</td><td>robOwnerShipInfos</td></tr>
 <tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>town</td><td>robOwnerShipInfos</td></tr>
 <tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>postcode</td><td>robOwnerShipInfos</td></tr>
 <tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>state</td><td>robOwnerShipInfos</td></tr>
 <tr><td>IC(OLD)</td><td>NO K/P(LAMA)</td><td>&nbsp;</td><td>&nbsp;</td><td>idCardNumber</td><td>robOwnerShipInfos</td></tr>
 <tr><td>IC(NEW)</td><td>NO K/P(BARU)</td><td>&nbsp;</td><td>&nbsp;</td><td>newIcNo</td><td>robOwnerShipInfos</td></tr>
 <tr><td>DATE OF BIRTH</td><td>TARIKH LAHIR</td><td>&nbsp;</td><td>&nbsp;</td><td>dob</td><td>robOwnerShipInfos</td></tr>
 <tr><td>RACE</td><td>BANGSA</td><td>&nbsp;</td><td>&nbsp;</td><td>race</td><td>robOwnerShipInfos</td></tr>
 <tr><td>GENDER</td><td>JANTINA</td><td>&nbsp;</td><td>&nbsp;</td><td>gender</td><td>robOwnerShipInfos</td></tr>
 <tr><td>NATIONALITY</td><td>KEWARGANEGARAAN</td><td>&nbsp;</td><td>&nbsp;</td><td>nationality</td><td>robOwnerShipInfos</td></tr>
 <tr><td>DATE JOIN</td><td>TARIKH MASUK</td><td>&nbsp;</td><td>&nbsp;</td><td>createDate</td><td>robOwnerShipInfos</td></tr>
</tbody></table>

## Page 3
<table class="tableizer-table">
<thead><tr class="tableizer-firstrow"><th>TITLE:</th><th>Information of previous owner(eng)</th><th>MAKLUMAT PEMILIK PERNIAGAAN TERDAHULU(MALAY)</th><th>&nbsp;</th><th>&nbsp;</th><th>Page 3</th></tr></thead><tbody>
 <tr><td>Column Name(English)</td><td>Column Name(MALAY)</td><td>&nbsp;</td><td>Remarks</td><td>json Node</td><td>Object Name</td></tr>
 <tr><td>Business Name</td><td>NAMA PERNIAGAAN</td><td>&nbsp;</td><td>&nbsp;</td><td>registrationName</td><td>robBusinessInfo</td></tr>
 <tr><td>Business Registrations No</td><td>NO.PENDAFTARAN PERNIAGAAN</td><td>&nbsp;</td><td>200803090077 (SA0085324-V)</td><td>registrationNo<br>checkDigit</td><td>robBusinessInfo</td></tr>
 <tr><td>12-digit new ?</td><td>&nbsp;</td><td>&nbsp;</td><td>200803090077</td><td>newFormatNo</td><td>GetNewFormatEntity</td></tr>
 <tr><td>Company No.</td><td>&nbsp;</td><td>&nbsp;</td><td>SA0085324</td><td>&nbsp;</td><td>&nbsp;</td></tr>
 <tr><td>Check Digit</td><td>&nbsp;</td><td>&nbsp;</td><td>V</td><td>&nbsp;</td><td>&nbsp;</td></tr>
 <tr><td>Name</td><td>NAMA</td><td>&nbsp;</td><td>This object took from list of robOwnershipListInfo with status != A .It means previous owner</td><td>ownerName</td><td>robOwnerShipInfos</td></tr>
 <tr><td>Residential Address</td><td>ALAMAT KEDIAMAN</td><td>&nbsp;</td><td>&nbsp;</td><td>address1</td><td>robOwnerShipInfos</td></tr>
 <tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>town</td><td>robOwnerShipInfos</td></tr>
 <tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>postcode</td><td>robOwnerShipInfos</td></tr>
 <tr><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>state</td><td>robOwnerShipInfos</td></tr>
 <tr><td>IC(OLD)</td><td>NO K/P(LAMA)</td><td>&nbsp;</td><td>&nbsp;</td><td>idCardNumber</td><td>robOwnerShipInfos</td></tr>
 <tr><td>IC(NEW)</td><td>NO K/P(BARU)</td><td>&nbsp;</td><td>&nbsp;</td><td>newIcNo</td><td>robOwnerShipInfos</td></tr>
 <tr><td>DATE OF BIRTH</td><td>TARIKH LAHIR</td><td>&nbsp;</td><td>&nbsp;</td><td>dob</td><td>robOwnerShipInfos</td></tr>
 <tr><td>RACE</td><td>BANGSA</td><td>&nbsp;</td><td>&nbsp;</td><td>race</td><td>robOwnerShipInfos</td></tr>
 <tr><td>GENDER</td><td>JANTINA</td><td>&nbsp;</td><td>&nbsp;</td><td>gender</td><td>robOwnerShipInfos</td></tr>
 <tr><td>NATIONALITY</td><td>KEWARGANEGARAAN</td><td>&nbsp;</td><td>REFER parameter ROB lookup.
English
select vchdescription where vchparametertype='ROBCitizenship' and vchcode='MAL'

MALAY
select vchdescription where vchparametertype='ROBCitizenshipMalay' and vchcode='MAL'</td><td>nationality</td><td>robOwnerShipInfos</td></tr>
 <tr><td>DATE JOIN</td><td>TARIKH MASUK</td><td>&nbsp;</td><td>&nbsp;</td><td>createDate</td><td>robOwnerShipInfos</td></tr>
 <tr><td>DATE OF WITHDRAWAL</td><td>TARIKH KELUAR</td><td>&nbsp;</td><td>&nbsp;</td><td>updateDate</td><td>robOwnerShipInfos</td></tr>
 <tr><td>REASON OF WITHDRAWAL</td><td>SEBAB KELUAR</td><td>&nbsp;</td><td>Refer to parameterROB.csv 
Sql (English) :
select vchdescription where vchparametertype='ROBB4Amend' and vchcode='D'

Sql (Malay) :
select vchdescription where vchparametertype='ROBB4AmendMalay' and vchcode='D'</td><td>ammendmentType</td><td>robOwnerShipInfos</td></tr>
</tbody></table>

<table class="tableizer-table">
<thead><tr class="tableizer-firstrow"><th>Stamp</th><th>&nbsp;</th><th>&nbsp;</th><th>&nbsp;</th><th>&nbsp;</th><th>For document with ctc</th></tr></thead><tbody>
 <tr><td>CTC QR Code</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td></tr>
 <tr><td>User ID</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td></tr>
 <tr><td>Printing Date with Time (Center)</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td></tr>
 <tr><td>Printing Date (Right Side)</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td></tr>
 <tr><td>Printing Date with Time (Bottom)</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td>&nbsp;</td><td></td></tr>
</tbody></table>