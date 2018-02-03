# utl_resizing_an_image_in_report_writing_interface
Resizing a jpeg Image for use in SAS Report Writing Interface.  Keywords: sas sql join merge big data analytics macros oracle teradata mysql sas communities stackoverflow statistics artificial inteligence AI Python R Java Javascript WPS Matlab SPSS Scala Perl C C# Excel MS Access JSON graphics maps NLP natural language processing machine learning igraph DOSUBL DOW loop stackoverfl SAS community.
    SAS Forum: Resizing a jpeg Image for use in SAS Report Writing Interface

    I suggest you use Python to resize and then include output in your SAS report.

    Input image
    https://goo.gl/NYTRwF
    https://github.com/rogerjdeangelis/utl_resizing_an_image_in_report_writing_interface/blob/master/utl_resizing_an_image_in_report_writing_interface_ba


    Output image - Resized Image (made it square)
    https://goo.gl/iSKtyf
    https://github.com/rogerjdeangelis/utl_resizing_an_image_in_report_writing_interface/blob/master/utl_resizing_an_image_in_report_writing_interface_ab

    Python PIL is a robust image processing package.
    Could not use WPS/Python because PIL is only supported in Python 2.7

    INPUT
    =====

      Web link
      https://images.pexels.com/photos/799443/pexels-photo-799443.jpeg?w=940&h=650&dpr=2&auto=compress&cs=...

      I saved it at

        d:/jpg/utl_resizing_an_image_in_report_writing_interface_input.jpg


    PROCESS ( all the code)
    =======================

      %utl_submit_py64("
        from PIL import Image;
        img = Image.open('d:/jpg/pexels-photo-799443.jpg');
        new_img = img.resize((500,500));
        new_img.save('d:/jpg/car_resized.jpg','JPEG', optimize=True);
      ");


    OUTPUT
    ======

      https://goo.gl/iSKtyf

    *                _              _       _
     _ __ ___   __ _| | _____    __| | __ _| |_ __ _
    | '_ ` _ \ / _` | |/ / _ \  / _` |/ _` | __/ _` |
    | | | | | | (_| |   <  __/ | (_| | (_| | || (_| |
    |_| |_| |_|\__,_|_|\_\___|  \__,_|\__,_|\__\__,_|

    ;

      https://images.pexels.com/photos/799443/pexels-photo-799443.jpeg?w=940&h=650&dpr=2&auto=compress&cs=...
      copied to

    *          _       _   _
     ___  ___ | |_   _| |_(_) ___  _ __
    / __|/ _ \| | | | | __| |/ _ \| '_ \
    \__ \ (_) | | |_| | |_| | (_) | | | |
    |___/\___/|_|\__,_|\__|_|\___/|_| |_|

    ;

    %utl_submit_py64("
      from PIL import Image;
      img = Image.open('d:/jpg/utl_resizing_an_image_in_report_writing_interface_ba.jpg');
      new_img = img.resize((500,500));
      new_img.save('d:/jpg/utl_resizing_an_image_in_report_writing_interface_ab.jpg','JPEG', optimize=True);
    ");
