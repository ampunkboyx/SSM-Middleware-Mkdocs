# DATA MAPPING ROB
## BUSINESS PROFILE
	Service	getBizProfile
PDF TEMPLATE		
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
<thead><tr class="tableizer-firstrow"><th>TITLE :</th><th>Business information (ENG)</th><th>Maklumat Perniagaan(Malay)</th><th>&nbsp;</th><th>&nbsp;</th><th>Page 1</th><th>&nbsp;</th></tr></thead><tbody>
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