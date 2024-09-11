# Add Document Time Stamp (DTS) to PDF document 

* **category**    diff
* **author**      Radek Svitak <radek@zetopry.cz>
* **source**      https://github.com/hidasw/TCPDF

## Description
The purpose of this repository is to store changes published in https://github.com/tecnickcom/TCPDF/pull/617#issuecomment-2315346099

## Example
````
$pdf=new TCPDF();
$pdf->setSignature('DTS-ONLY', file_get_contents('postsignum_tsa_tsu1.pem'), '', '', 1, []);
$pdf->setTimeStamp(TSA_URL, TSA_USERNAME, TSA_PASSWORD);
$pdf->loadHtml($html);
$pdf->setSignatureAppearance(20,10,50,15);
$output=$pdf->Output($filename,'S');
````
Result displayed in Adobe Acrobat:

![obrazek](https://github.com/user-attachments/assets/b020c5a7-7240-4144-808f-5ca24527f34f)


## Developer(s) Contact

* Radek Svitak <radek@zetory.cz>
