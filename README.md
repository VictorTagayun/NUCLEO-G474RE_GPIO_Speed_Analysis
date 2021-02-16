## NUCLEO-G474RE_GPIO_Speed_Analysis

### 2021-02-17  
Release compile made it Faster from 21.3 Mhz to 34 Mhz  

comparing  
    GPIOA->BSRR = (1<<8);  
    GPIOA->BSRR = (1<<(8+16));  
and  
	  GPIOA->BSRR = (1<<8); // Set  
	  GPIOA->BRR = (1<<8); // Reset
