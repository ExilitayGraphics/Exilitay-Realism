Exilitay Realism II - New Changes / Fixes (App v2.1)

TONEMAPPING:  
• Tone taillights going pink in high exposure fix  
• Tone bloomy taillights fix  
• Tone red cores are brighter and keep their color, instead of looking grey/washed out  
• Filmic taillights looking washed out in high exposure fix  
• Filmic reds are slightly less saturated & deeper  
• Filmic red channel and emissive cores are deeper & brighter  
• Filmic has slightly more highlights, stronger s-curve & shadows  
• Filmic color volume eases off for highlight peaks  
• Filmic blues are a little darker and less saturated, so they don't go teal  
• Filmic reds are deeper at higher color volume  
• Filmic daytime taillights are slightly more orange and less saturated  
• Clouds stay out of color volume, so they keep more of their natural white color  
• Highlight compression no longer reduces emissive cores  
• Taillights no longer clip from high exposure

COLOR:  
• Color Engine 'Photo Realism' is slightly less bright  
• Exilitay Spec day sepia is about 50% lower  
• Exilitay Spec temp is slightly cooler for LCS & Gamma
• All color grades reworked for a more natural, realistic look  
• Added new color grades: Natural & Tokyo  
• Removed Chroma. Natural is now the default color grade

SUN BLINDING:  
• Sun going through objects fix  
• Refined the defaults for a more natural look  
• Pure's sunblinding is automatically disabled when mine is enabled (Gamma fix)

EXPOSURE:  
• Removed bad weather AE Adapt boost, so it no longer over-exposes for certain weather/scenes  
 Rainy/overcast weather keeps a more balanced exposure  
• AE Adapt no longer spikes when driving into a tunnel  
• Tunnel blinding exposure is now only for real tunnels, not bridges or underpasses  
 This was causing exposure flashes when driving under bridges (with high tunnel blinding strength)  
• Auto exposure will still increase under bridges/underpasses  
• Sky Occlusion Exposure is separate from tunnel exposure/blinding  
• AE Adapt is weaker under bridges, underpasses & tunnels to prevent over-exposure  
• AE Adapt has a different meter for lower sun angles for more accurate exposure correction  
• AE Adapt no longer brightens some scenes that were already bright (Gamma fix)  
 A bright day scene now slightly reduces exposure. A normal scene can rise a little
 
LIGHTING:  
• Increase in ambient lighting for softer, natural lighting during day  
• Significant ambient lighting changes to overcast/bad weather & foggy weather  
• More ambient light & daylight for heavier foggy/bad weather - was too dark before  
• Emissive lights are doubled in strength for bad weather/foggy weather  
• Ambient saturation was lowered as ambient lighting/shadows were too blue  
• Overcast and bad weather drop world brightness to about 60% (LCS)  
 Scene brightness drops about 15%  
• Fixed distant street lights appearing bloomy bug

FOG:  
• Sun showing for 'Fog' weather fix (Gamma)  
 This also caused unnatural sun reflections  
• Sun level & speculars fall for foggy weather  
 lighting is more natural, relying more on ambient light  
• Fog density is 50% stronger for 'Fog' weather  
• Fog weather is also brighter for LCS  
• More Fog ambient lighting for Gamma
TUNNEL FOG DIMMER:  
• Fog smoothly appears just before the tunnel exit  
 Before it would appear after exiting and looked unnatural  
• Short tunnels keep most of the fog  
• Heavy fog takes slightly longer to clear inside a tunnel  
 Added the delay as short tunnels would clear the fog too soon
 
BLOOM:  
• Glare Boost is now Bloom Boost (day, night, bad weather, and fog)  
• It raises bloom, widens it, and slightly lowers the threshold (doesn't boost glare)  
• In fog or bad weather, the day and night bloom boost weakens, so it doesn't stack with the day/night boost  
• Exposure Bloom is extra bloom for over-exposure (Gamma)  
 It widens the bloom and lowers the threshold. It does not raise glare
 
REFLECTIONS:  
• Reflections in occlusion were reduced  
 They were too strong in tunnels, causing an unnatural visual change  
• Bad weather no longer has a reflection level boost  
• Reflection saturation and polariser filter are lower  
• Reflection emissive boost raised (Gamma)

EXILITAY FX:  
• Filmic Sharpen doesn't sharpen over depth-of-field blur, so the blur no longer becomes grainy  
• Filmic Sharpen and Local Contrast both fade out with distance (so distant objects are softer)  
• Filmic Sharpen skips emissives and their reflections, so they don't create a halo  
• Changes to how bright/dark areas are affected for Sharpen and Local Contrast (more balance)  
• Chromatic Aberration no longer clears the depth-of-field blur  
• Chromatic Aberration rebuilt  
 CA Intensity, CA Radius, and Lens Edge Blur are removed  
• Depth of field blur is smoother and higher quality  
 It runs at half resolution, so it's more optimised, but the blur itself is stronger  
• The sharp texture in the blur is fixed  
• DOF Bokeh Softness is removed  
• Lens distortion defaults are more subtle  
• Film grain defaults are retuned; default mode is monochrome

VR  
• Compatibility for VR has been added (supporting both LCS & Gamma)

APP:  
• App settings not syncing after changing ppfilters or restarting WeatherFX fix  
• App UI redesigned with a cleaner, more user-friendly interface  
• New license page with a simple step-by-step activation guide  
• Custom presets are easier to use, with Load and Delete on each preset  
• New Factory Preset in the style of a Dashcam  
• All Factory Presets have been retuned (Gamma & LCS)  
• New accent colour option in Settings (Orange, Blue or Green)  
• New Color Grade Preview window. Compare on/off or A/B
