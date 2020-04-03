# PIC32 version 3.21 - RedBird_ThinkiFy_4.7.1_Support 
PIC32 FW changed to accommodate ThinkiFy 4.7.1 FW

Changes

1. Added command SM1 
2. Changed PC32 Intrupt as per ThinkiFY FW 4.7.1
3. Changed P command from P131 to P023 - As per Curt's Recommendation 
4. Changed command GG0 to GG01 - GG1 is not working in TF FW 4.7.1
5. Added commands
      IQ0  = Set Q to 0 Q=0x0
      II1 = Set inner loop to (default) = INNERLOOP=0x01
      IW1 =  Select loop 1 (default) = SELECTLOOP=0x1
      MR = just the reset default of SELECTALL on mask 0
6. RO0 is replaced with RO1
7. Changed TR65TriggerLen = 9 // This giving 9msec to PIC to settle ThinkiFy to build RF power and not to miss tag. This is possible with new thinkify FW because new FW is need lesser hold time to compare to 4.0.1 version of thinify FW and hence has no impact on over all process
