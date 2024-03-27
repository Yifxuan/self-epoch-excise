# self-epoch-excise
begin:constant
  laser_lamada     = 0.8 * micron       
  laser_omega      = 2.0*pi*c/laser_lamada      
  laser_period     = laser_lamada/c      
  laser_k          = 2*pi/laser_lamada         

  x_spot           = 5 * micron       

  w0               = 11 * micron           

  rayleigh_length  = pi*w0^2/laser_lamada          
  wz               = w0*sqrt(1+(x_spot/rayleigh_length)^2)    
  radius_curv      = x_spot*(1.0+(rayleigh_length/x_spot)^2)    
  gouy = atan(x_spot/rayleigh_length)         
  

  ad0              = 1.9      
  Intensity        = (1.37*10^18)*ad0^2/((laser_lamada^2)*10^12)     
  n_crit           = 1.1*10^27/((laser_lamada^2)*10^12)     
  T0               = laser_lamada/c     
  las_t_fwhm1      = 45 * femto      
  nc               = n_crit     
  
end:constant
