---
sidebar_position: 2
---

# 📚 Thông số làm xe

Thông số làm xe

## CẤM NHỮNG THỨ SAU

1. Cửa ảo, Xuống xe nhanh quá quy định , Tầm nhìn xa
2. Chống đạn full xe , Chống đạn gầm , Bắn không hư ( Tất cả chỗ có kính đều phải bắn xuyên , Không chống đạn càng gió, Spoiler )
3. Chống lật , Khung ảo, Dốc ảo, Chạy xuyên vật thể, Chạy quá dính đường

## VỀ FILE CARCOL + VEHICLE

1. Tất cả các mức độ xe tối đa là 100 ( ENGINE, ARMOUR.. )
2. Vehicle Class chỉ được để VC_SUPER hoạc VC_SPORT
3. Không được thêm các Flags bịp trong cả file Handling và Vehicle (FLAG_RAMP ... )

## FILE KHÁC

1. File YTD + YFT của xe không được quá 32Mib ( Trường hợp xe nhiều decal sẽ liên hệ riêng với ADMIN để được chấp thuận )
2. COL và TRỤC XE sẽ như hình bên dưới, TRỤC XE không được thấp hơn giữa bánh xe trở xuống

:::note

Trục xe phải đúng quy định , nếu trục xe khác hãy liên hệ admin để được cho phép hay không

:::

![image](https://r2.fivemanage.com/40OTy1Wf8i90yD29Jzidw/Screenshot2025-10-19145351.png)

:::important

thông số render LOD của xe phải theo quy tắc dưới để tránh lag , cái này sửa trong file meta của xe

* 100m full
* 150m low
* 300m ẩn

:::

# HANDLING XE ĐỘC QUYỀN

1. slot cư dân
2. slot xe hỗ trợ gang và ban ngành thì phải làm thêm theo như bảng thứ 2
3. Tốc độ tăng tốc của xe tối đa từ 0 - 400km nằm trong khoản 20-30S ( từ cầu casino đến ngang nhà tù )
4. Vì thông số mỗi chiếc xe tuy giống nhau nhưng tốc độ sẽ không hoàn toàn giống nên ADMIN sẽ cang thiệp nếu chiếc xe đó có dấu hiệu OP hơn những xe khác
5. Sẽ tiếp tục update handling nếu có nhiều vấn đề với member

:::warning

đây là thông số dành cho xe độc quyền , xe hỗ trợ , xe chủ gang

:::

```xml title="handling.meta"
<fMass value="3000.0" />                                              
<fInitialDragCoeff value="3.0" />                                     
<fDownforceModifier value="25" />                     <!-- Tối đa 25-->
<fPercentSubmerged value="85.0" />                               
<vecCentreOfMassOffset x="0.00" y="0.0" z="0.0" />    <!-- Z = 0 -->
<nInitialDriveGears value="7" />                      <!-- Tối đa 7 -->
<fInitialDriveForce value="0.4" />                 <!-- Tối đa 0.4 -->
<fDriveInertia value="1.0" />                                    
<fClutchChangeRateScaleUpShift value="8.0" />                       
<fClutchChangeRateScaleDownShift value="8.0" />                     
<fInitialDriveMaxFlatVel value="400" />         <!-- Tối đa 400 -->
<fBrakeForce value="5.0" />                       <!-- Tối đa 5.0 -->
<fHandBrakeForce value="0.5" />                  <!-- Tối đa 10.0 -->
<fSteeringLock value="45.0" />                   <!-- Tối đa 60 -->
<fTractionCurveMax value="6.0" />                <!-- Tối đa 10 -->
<fTractionCurveMin value="6.0" />                 <!-- Tối đa 10 -->
<fLowSpeedTractionLossMult value="0.0" />                          
<fTractionLossMult value="0.0" />                                
<fSuspensionForce value="2.2" />                                  
<fSuspensionCompDamp value="1.5" />                               
<fSuspensionReboundDamp value="1.5" />                                                            
<fCollisionDamageMult value="0.3" />                                 
<fWeaponDamageMult value="0.3" />                                  
<fEngineDamageMult value="0.3" />                              
<strModelFlags>440010</strModelFlags>                                     
<strHandlingFlags>20002</strHandlingFlags>                             
<SubHandlingData>
  <Item type="NULL" />
  <Item type="NULL" />
  <Item type="NULL" />
</SubHandlingData>
```

## HANDLING XE GANG

1. đây là xe được tặng 10 chiếc khi lên gang
2. đối với xe gang thì chỉ được làm mỗi led tĩnh và decal phát sáng , còn lại là zin và không có gì cả
3. Tốc độ tăng tốc của xe tối đa từ 0 - 300km nằm trong khoản 20-30S
4. Vì thông số mỗi chiếc xe tuy giống nhau nhưng tốc độ sẽ không hoàn toàn giống nên ADMIN sẽ cang thiệp nếu chiếc xe đó có dấu hiệu OP hơn những xe khác
5. Sẽ tiếp tục update handling nếu có nhiều vấn đề với member

:::warning

đây là thông số dành cho xe gang cấp nhiều chiếc

:::

```xml title="handling.meta"
<fMass value="3000.0" />                                              
<fInitialDragCoeff value="3.5" />                                     
<fDownforceModifier value="10" />                     <!-- Tối đa 10 -->
<fPercentSubmerged value="85.0" />                               
<vecCentreOfMassOffset x="0.00" y="0.0" z="0.0" />    <!-- Z = 0 -->
<nInitialDriveGears value="5" />                      <!-- Tối đa 6 -->
<fInitialDriveForce value="0.4" />                 <!-- Tối đa 0.4 -->
<fDriveInertia value="1.0" />                                    
<fClutchChangeRateScaleUpShift value="6.0" />                       
<fClutchChangeRateScaleDownShift value="6.0" />                     
<fInitialDriveMaxFlatVel value="250.0" />         <!-- Tối đa 250 -->
<fBrakeForce value="3.0" />                       <!-- Tối đa 3.0 -->
<fHandBrakeForce value="5.0" />                  <!-- Tối đa 5.0 -->
<fSteeringLock value="45.0" />                   <!-- Tối đa 60 -->
<fTractionCurveMax value="6.0" />                <!-- Tối đa 7 -->
<fTractionCurveMin value="6.0" />                 <!-- Tối đa 7 -->
<fLowSpeedTractionLossMult value="0.0" />                          
<fTractionLossMult value="0.0" />                                
<fSuspensionForce value="2.2" />                                  
<fSuspensionCompDamp value="1.5" />                               
<fSuspensionReboundDamp value="1.5" />                                                             
<fCollisionDamageMult value="0.3" />                                 
<fWeaponDamageMult value="0.3" />                                  
<fEngineDamageMult value="0.3" />                              
<strModelFlags>440010</strModelFlags>                                     
<strHandlingFlags>20002</strHandlingFlags>                             
<SubHandlingData>
  <Item type="NULL" />
  <Item type="NULL" />
  <Item type="NULL" />
</SubHandlingData>
```

## VỀ VEHICLELAYOUT

1. Giá trị trong tối đa là 1.1 đối với xe gang , 1.3 đối với xe độc quyền
2. xe mà layout bịp lạm dụng thì sẽ bị blacklist đến khi sửa xong