#############################################################################################################################################
#  USAGE :                                                                                                                              
#       python3 VPOT.py  -  will return a help screen                                                                                    
#       python3 VPOT.py priority <location for output file+prefix> <file of input VCF files>      will create a default parameter file     
#       python3 VPOT.py priority <location for output file+prefix> <file of input VCF files> <parameter file>                          
#       python3 VPOT.py genef <location for output file+prefix> <VPOT prioritiy output> <gene list>                                  
#       python3 VPOT.py samplef <location for output file+prefix> <VPOT prioritiy output> <sample selection file>                   
#                                                                                                                                

##############################################################################################################################################
# Prioritise your variants (VCF/TXT input)                                                                                           
# 
#          	python3 VPOT.py priority <location for output file+prefix> <file of input VCF files> <parameter file>                    
#                                                                                                                                       
# command :                                                                                                                             
#           change to test_data directory
#
# For VCF-	python3 ../VPOT.py priority testout_ test_VCF_sample_list.txt test_variants_parameters.txt                                
#
#       	files FAM_1.vcf, test_VCF_sample_list.txt and test_variants_parameters.txt are supplied in the test_data directory of VPOT download  
#
# For TXT-	python3 ../VPOT.py priority testout_ test_TXT_sample_list.txt test_variants_parameters.txt                           
#
#         	files FAM_1.txt and test_TXT_sample_list.txt are supplied in the test_data directory of VPOT download                              
#                                                                                                                                             
# result : an output file will be created                                                                                                   
#          testout_final_output_file_XXXXXXXXXX.txt                                                                                            
#                                                                                                                                              
#################################################################################################################################################
#
#################################################################################################################################################
# Filter your output by gene list                                                                                                         
#
#       	python3 VPOT.py genef <location for output file+prefix> <VPOT prioritiy output> <gene list>                                  
#                                                                                                                                                
# command :                                                                                                                                        
#          	change to test_data directory
#
# 			python3 ../VPOT.py genef testout_ testout_final_output_file_XXXXXXXXXX.txt test_gene.txt                                               
#
#         	file test_gene.txt is supplied in the test_data directory of VPOT download                                                               
#                                                                                                                                                  
# result : an output file will be created                                                                                                          
#          testout_gene_filtered_output_file_XXXXXXXXXX.txt                                                                                        
#                                                                                                                                                  
###################################################################################################################################################
#
###################################################################################################################################################
# Filter your output by sample pedigree                                                                                                           
#                                                                                                                                                 
#       	python3 VPOT.py samplef <location for output file+prefix> <VPOT prioritiy output> <sample selection file>                   
#
# command :                                                                                                                                       
#       	change to test_data directory
#
# 			python3 ../VPOT.py samplef testout_ testout_final_output_file_XXXXXXXXXX.txt test_sample_set.ped                                      
#
#         	file test_sample_set.ped is supplied in the test_data directory of VPOT download                                                        
#                                                                                                                                                  
# result : an output file will be created                                                                                                          
#          testout_variant_filtered_output_file_XXXXXXXX.txt                                                                                       
#                                                                                                                                                  
###################################################################################################################################################