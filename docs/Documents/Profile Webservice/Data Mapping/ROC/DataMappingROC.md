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
# DATA MAPPING ROC


## COMPANY PROFILE

## Page 1
<table class="tableizer-table">
	<thead>
		<tr class="tableizer-firstrow">
			<th>TITLE :</th>
			<th>Company information (ENG)</th>
			<th>MAKLUMAT SYARIKAT(Malay)</th>
			<th>&nbsp;</th>
			<th>&nbsp;</th>
			<th>&nbsp;</th>
			<th>&nbsp;</th>
			<th>&nbsp;</th>
			<th>&nbsp;</th>
			<th>&nbsp;</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Column Name(English)</td>
			<td>Column Name(MALAY)</td>
			<td>Sample Data</td>
			<td>Remarks</td>
			<td>Webservice</td>
			<td>json Node / Parameter</td>
			<td>Object Name</td>
			<td>Sdn Bhd</td>
			<td>CLBG</td>
			<td>Foreign</td>
		</tr>
		<tr>
			<td>Company Name</td>
			<td>Nama Syarikat</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>companyName</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Last Old Name</td>
			<td>Nama Syarikat Lama</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>companyOldName</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Date of Change</td>
			<td>Tarikh Pertukaran</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>dateOfChange</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Registration No.</td>
			<td>No. Pendaftaran</td>
			<td>&nbsp;</td>
			<td>201101006232(934369-T)</td>
			<td>GetCompProfile</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>12 digit new ?</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>201101006232</td>
			<td>GetNewFormatEntityNo</td>
			<td>NewFormatNo</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Company Number</td>
			<td>No Syarikat</td>
			<td>&nbsp;</td>
			<td>should show e.g :84984-H</td>
			<td>GetCompProfile</td>
			<td>companyNo-checkDigit</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Check Digit</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>T</td>
			<td>GetCompProfile</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Incorporation Date</td>
			<td>Tarikh Penubuhan</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>incorpDate</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Registration Date</td>
			<td>Tarikh Pendaftaran</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>registrationDate</td>
			<td>rocCompanyInfo</td>
			<td>No</td>
			<td>No</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Jenis</td>
			<td><b>English</b>
				<br> B - LIMITED BY SHARE AND GUARANTEE,
				<br> G - LIMITED BY GUARANTEE
				<br> S - LIMITED BY SHARES
				<br> U - UNLIMITED
				<br> <b>Malay</b>
				<br> B - BERHAD MENURUT SAHAM DAN JAMINAN,
				<br> G - BERHAD MENURUT JAMINAN
				<br> S - BERHAD MENURUT SYER
				<br> U - TIDAK TERHAD</td>
			<td>"Base from pdf template : column type is combination of Type :companyType :companyStatus"</td>
			<td>GetCompProfile</td>
			<td>companyType</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Jenis</td>
			<td>R-Private Limited (eng);Syarikat Persendirian(Malay)
				<br> U-Public Limited(eng);Syarikat Awam(Malay)</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>companyStatus</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Status</td>
			<td>Status</td>
			<td>B - DISSOLVED CONVERSION TO LLP
				<br> C - CEASED BUSINESS
				<br> D - DISSOLVED
				<br> E - EXISTING
				<br> R - REMOVED
				<br> W - WINDING UP
				<br> X - NULL AND VOID BY COURT ORDER
				<br> Y - STRUCK-OFF & WINDING-UP VIA COURT ORDER</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>statusOfCompany</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>LLP NAME</td>
			<td>NAMA PLT</td>
			<td>&nbsp;</td>
			<td>* need to view if status is Dissolved- Conversion to LLP</td>
			<td>GetCompProfile</td>
			<td>llpName</td>
			<td>rocCompanyInfo</td>
			<td>No</td>
			<td>No</td>
			<td>No</td>
		</tr>
		<tr>
			<td>LLP NUMBER</td>
			<td>NOMBOR PLT</td>
			<td>&nbsp;</td>
			<td>* need to view if status is Dissolved- Conversion to LLP</td>
			<td>GetCompProfile</td>
			<td>llpNo</td>
			<td>rocCompanyInfo</td>
			<td>No</td>
			<td>No</td>
			<td>No</td>
		</tr>
		<tr>
			<td>CONVERSION DATE</td>
			<td>TARIKH PERTUKARAN</td>
			<td>&nbsp;</td>
			<td>* need to view if status is Dissolved- Conversion to LLP</td>
			<td>GetCompProfile</td>
			<td>llpconvertDate</td>
			<td>rocCompanyInfo</td>
			<td>No</td>
			<td>No</td>
			<td>No</td>
		</tr>
		<tr>
			<td>Registered Address</td>
			<td>Alamat daftar</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>address1</td>
			<td>rocRegAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>address2</td>
			<td>rocRegAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>address3</td>
			<td>rocRegAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>town</td>
			<td>rocRegAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>state</td>
			<td>rocRegAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Postcode</td>
			<td>Poskod</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>postcode</td>
			<td>rocRegAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>Origin</td>
			<td>Tempat Penubuhan</td>
			<td>MAL- Malaysia</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>companyCountry</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>Business Address</td>
			<td>Alamat Perniagaan</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>address1</td>
			<td>rocBusinessAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>address2</td>
			<td>rocBusinessAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>address3</td>
			<td>rocBusinessAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>town</td>
			<td>rocBusinessAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>state</td>
			<td>rocBusinessAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>Postcode</td>
			<td>Poskod</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>postcode</td>
			<td>rocBusinessAddressInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>Nature of Business</td>
			<td>Jenis Perniagaan</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>GetCompProfile</td>
			<td>businessDescription</td>
			<td>rocCompanyInfo</td>
			<td>Yes</td>
			<td>Yes</td>
			<td>Yes</td>
		</tr>
	</tbody>
</table>

## Page 2
## Page 3
## Page 4
## Page 5
## Page 6


<!-- <iframe width="880" height="664" frameborder="0" scrolling="no" src="https://ssmmy.sharepoint.com/sites/UnitPembekalanData/_layouts/15/Doc.aspx?sourcedoc={0d607c4b-c44c-403b-a205-32b6a21ad5b5}&action=embedview&wdAllowInteractivity=False&wdHideGridlines=True&wdHideHeaders=True&wdDownloadButton=True&wdInConfigurator=True"></iframe> -->