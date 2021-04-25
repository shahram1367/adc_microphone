# adc_microphone
         ADC with DMA 
        input: analog input(microphoe)
        output: LEDs set and reset selected as output (digital output)
 		
		if( adc_Result < 1241 ){
		HAL_GPIO_TogglePin(user_1_GPIO_Port, user_1_Pin);
					}
		if((adc_Result >= 1241) && (adc_Result < 2482))
		{
		HAL_GPIO_TogglePin(user_2_GPIO_Port, user_2_Pin);
		}
		
		if(adc_Result >= 2482)
		{
			HAL_GPIO_TogglePin(user_3_GPIO_Port, user_3_Pin);
		}
		HAL_Delay(1);
  
	
