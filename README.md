# PDF-crop
just simple cropping PDF using imagemagick


This is not a code. this is only command line to reuse in future.	

*process
1) PDF -> JPG(with cropping) -> PDF

*command line code 	
1. convert PDF to jpg sequence files	
	convert -geometry 1600x1600 -density 200x200 -quality 100 -crop (doc_width)+(doc_height)-(doc_width)-(doc_height) &PDF_filename.pdf &target_filename.%04d.jpg	
2. ZIP the jpg sequence as PDF	
convert *.jpg -compress Zip output.pdf

*Issues 				
"PDF is editable" is an idiot's idea.

