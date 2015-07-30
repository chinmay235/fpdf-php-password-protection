# fpdf-php-password-protection
Password Protection using FPDF



    <?php
    require('fpdf_protection.php');
    
    $pdf=new FPDF_Protection();
    $pdf->SetProtection(array('print'),'password');
    //$pdf->SetProtection(array('print'));
    $pdf->AddPage();
    $pdf->SetFont('Arial');
    $pdf->Write(10,'You can print me but not copy my text.');
    $pdf->Output();
    ?>
    
    
    


