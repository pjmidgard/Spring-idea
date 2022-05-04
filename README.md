# Spring-idea
Sping-idea
                                    Equal_info_between_of_the_cirlce_of_the_file=Equal_info_between_of_the_cirlce_of_the_file_2

                                    
                                    if   Circle_times2==0 and SpinS==0:
                                    	Equal_info_between_of_the_cirlce_of_the_file="1"+Equal_info_between_of_the_cirlce_of_the_file
                                    	SpinS=1

                                    lenf6=len(Equal_info_between_of_the_cirlce_of_the_file)                      
                                    Equal_info_between_of_the_cirlce_of_the_file_17=""
                                
                                    Equal_info_between_of_the_cirlce_of_the_file=Equal_info_between_of_the_cirlce_of_the_file_2
                                    
                                    lenf6=len(Equal_info_between_of_the_cirlce_of_the_file)
                                
                                    add_bits=""

                                    Times_6=""

                                    #Compression

                                    sda10=""
                                    Translate_info_Decimal=""
                                    
                                    Equal_info_between_of_the_cirlce_of_the_file_17=""
                 
                                    

                                    if Circle_times2>=(2**8)-2:
                                            compress_or_not_compress=2

                                    lenf6=len(Equal_info_between_of_the_cirlce_of_the_file)
                                            
                                    
                                    Find_center_info=Equal_info_between_of_the_cirlce_of_the_file

                                    block=0
                                    Find_Save=1
                                    Find_Save4=0
                                    
                                    block2=0
                                    Find_center_top=""

                                    while block<lenf6:

                                           Find_center_info1=Find_center_info[block:block+6]
                                           Find_center_info2=Find_center_info[block:block+5]
                                           

                                           if Find_center_info1=="111111" and Find_Save==1:
                                                Find_center_info=Find_center_info[:block]+Find_center_info[block+6:]
                                                Find_center_top=Find_center_top+"000000"
                                                
                                           
                                           elif Find_Save==1:
                                                Find_center_info=Find_center_info[:block]+Find_center_info[block+5:]
                                                Find_center_top=Find_center_top+Find_center_info2

                                                   
                                           elif Find_center_info1=="000000" and Find_Save4==0 and Find_Save==5:
                                                    Find_Save_binary=bin(Find_Save)[2:]
                                                    lenf=len(Find_Save_binary)

                                                    add_bits8=""
                                                    count_bits=5-lenf%5
                                                    z=0
                                                    if count_bits!=0:
                                                        if count_bits!=5:
                                                                while z<count_bits:
                                                                        add_bits8="0"+add_bits8
                                                                        z=z+1

                                                    Find_center_info3=add_bits8+Find_Save_binary
                                                    check_numner_equal=add_bits8+Find_Save_binary
                                                    
                                                    Find_Save4=1
                                                    if check_numner_equal!=Find_center_info2:
                                                            
                                                            #print(check_numner_equal)
                                                            Find_center_info=Find_center_info[:block]+Find_center_info[block+6:]
                                                            Find_center_top=Find_center_top+Find_center_info3
                                                    elif check_numner_equal==Find_center_info2:
        
                                                            Find_center_info=Find_center_info[:block]+Find_center_info[block+5:]
                                                            Find_center_top=Find_center_top+"111111"
                                                        
                                                            
                                                            
                                                    
                                           Find_Save=Find_Save+1
                                           if Find_Save==30:
                                                   Find_Save=1
                            
                                                   Find_Save4=0
                                                   
                                           block=block+6
                                     
                                    center_top=len(Find_center_top)
                                          
                                    long_top_comperession=bin(center_top)[2:]
                                    lenf=len(long_top_comperession)

                                    add_bits7=""
                                    count_bits=32-lenf%32
                                    z=0
                                    if count_bits!=0:
                                        if count_bits!=32:
                                                while z<count_bits:
                                                    add_bits7="0"+add_bits7
                                                    z=z+1   
                                          
                                    Equal_info_between_of_the_cirlce_of_the_file_17=add_bits7+long_top_comperession+Find_center_top+Find_center_info
                                    lenfS=len(Equal_info_between_of_the_cirlce_of_the_file_17)
                                    #print(lenfS)
                                    
                                    if lenf6<=lenfS:
                                        Deep3=lenfS
