# Spring-idea
Sping-idea

block=0
                                                    Find_Save=1
                                                    Find_Save4=0
                                                    Find_Save5=0
                                                    block2=0

                                                    while block<lenf6:

                                                           Find_center_info1=Find_center_info[block:block+6]
                                                           Find_center_info2=Find_center_info[block:block+5]
                                                           Find_center_info3=Find_center_info[block2:block2+6]

                                                           if Find_center_info3=="000000" and Find_Save5==0:
                                                                Find_center_info=Find_center_info[:block2]+"111111"+Find_center_info[block2+6:]
                                                                
                                                               
                                                          
                                                                  
                                                                   
                                                           if Find_Save4==0 and Find_Save5==0:
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
                                                                    if check_numner_equal==Find_center_info2:
                                                                            Find_center_info=Find_center_info[:block]+"000000"+Find_center_info[block+6:]
                                                                          
                                                                    elif check_numner_equal=="111111":
                                                                            Find_center_info=Find_center_info[:block2]+Find_center_info[block2+6:]
                                                                            Find_center_info=Find_center_info[:block2]+Find_center_info[block2+6:]
                                                                            Find_Save5=1
                                                                            

                                                                         
                                                           
                                                                            
                                                                            
                                                                            
                                                                    
                                                           Find_Save=Find_Save+1
                                                           if Find_Save==30:
                                                                   Find_Save=1
                                                                   block2=block
                                                                   Find_Save4=0  
                                                           block=block+6
