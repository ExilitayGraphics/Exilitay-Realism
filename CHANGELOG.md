Exilitay Realism II - Changelogs

TONEMAPPING:
Exilitay-Filmic (formerly GT7-Blend)
• Brighter highlights, darker shadows, and deeper colors than Tone
• Hue Preserve, highlight compression, and midtone shaping
• Removed GT-Film tonemap
Exilitay-Tone
• Softer, more natural/photographic look
• Lifted midtones
Separate Night Tonemap
• Own Filmic and Tone curves for day and night
• Off = night uses the day curve

Highlights
• Stronger highlights overall
• Highlights Compression prevents sun & taillight cores (overall white peaks) from clipping
• Highlights Desaturation only hits the hottest whites/sun, and keeps them bright so the sun doesn't go grey
• Hue Preserve keeps clipped colors accurate (e.g. sun speculars on car paint) instead of going white/grey
Shadows & midtones
• Darker shadows overall
• Subtle Shadow Lift only on dark blacks (to prevent crushed blacks)
• Lower midtone gamma for richer, less washed midtones
• Tone stronger S-Curve for extra contrast in the midtones
• Tone Shadow Density for softer shadows
Color Volume (Filmic)
• Retuned for deeper, richer colors
• Richer colors fade at very bright highlights, so colors stay deep without the colors clipping
• blue channel saturation handled separately so the sky doesn't go teal
Other tonemap changes
• Tailights/LEDs are less hot. Less desaturation from 1.09, so the core stays the true color
  Weaker lamps were losing their color. That brightness gate is off
• Cleaner RGB curve for more accurate colors

Filmic = punchy/cinematic, Tone = softer/photographic


EXPOSURE:
Two modes: Camera-like & Eye-like. 
Camera-like is slightly more over-exposed. Eye-like is more natural and less bright in most scenarios
Camera-like (More reactive overall)
• Smaller/centre-weighted meter (the car and a small area around you)
• You can resize it: smaller = closer to spot metering, larger = closer to full-frame
• Holds exposure on the subject instead of letting the sky pull it down
• AE Adapt: shade/dark scenes lift the CBE exposure, open sun slightly reduces CBE
• Exposure reacts faster than it darkens, so it brightens quickly in the shade, but doesn't react as fast when scene becomes brighter
• Show Metering Area draws the metering area on screen
Eye-like (Smoother & more balanced)
• Wider, evaluative meter (more of the surroundings)
• Darker and more even/balanced, like how your eyes adapt to the whole scene rather than exposing for just the subject
• No AE Adapt, so it stays even instead of exposing just for the subject
• Darkens faster than it brightens, so bright scenes don't blow out as quickly, and dark scenes take slightly longer to increase


EXILITAY FX: 
Local Contrast
• Clarity is removed. Local Contrast replaces the effect
• Bright areas get more LC, dark areas a bit less, to prevent over-contrast on dark objects (more balanced)
• Threshold fades with distance (so distant objects stay soft)
• Skips sun & emissives to prevent halos around lamps/sun
Filmic Sharpen
• Replaced Luma Sharpening
• Filmic Sharpen does a better job at sharpening the bright edges as well as dark (more balanced)
DEPTH OF FIELD:
• Circle of Confusion (CoC) from Ilja (Photo-mode CSP)
• 3rd person focuses the car as the subject. For 1st person, the cockpit is blurred (can be inverted)
• Windscreen height stays locked in cockpit to prevent Auto DOF from being inaccurate due to NeckFX movement

OTHER EXILITAYFX CHANGES:
• CA Intensity, CA Radius, and CA Blur (skips the sun and emissives)
• Separate Lens Edge CA for the corners, plus a separate corner blur
• Smaller lines stay weaker than wide edges
Film Grain
• Split for day and night, with size and softness. 1.09 was one amount
• Color or monochrome mode (colored or black & white)
Color Engine
• PhotoRealism & Vibrance retuned + new Exilitay-Spec Preset
• Master Vibrance (red channel vibrance is reduced)
Removed
• Dashcam VHS
• Sky color-grading


LIGHTING & WEATHER:
World lighting
• Facing the sun raises the sun level slightly
• Sun behind the camera is pulled down so it doesn't overexpose (especially for white cars)
• Speculars are also stronger when facing the sun, and weaker when the sun is behind the camera
• Sky level fades to 0 once sun is below horizon, so the horizon doesn't stay white (Gamma)
Clouds & overcast
• Overcast/bad weather: more ambient and sun light, retuned clouds-shadow levels
• Bad-weather color: a bit less saturation, slightly cooler & more sepia


TUNNELS & OCCLUSION:
• Custom occlusion from sky samples + roof height
• Sky Occlusion is overhead only (overpasses/bridges)
Occlusion Ambient + Sun Dimmer
• Decreases ambient light for occlusion & sky occlusion, and sun level for tunnels only - Stronger for LCS
• 500ms delay to prevent a passing sign/street lamp or other object reading as a roof
  Both work at the same time, but only the stronger one is used. Sky Occlusion dims less than a full tunnel (and has less exposure boost)
Tunnel Fog Dimmer
• Decreases fog inside tunnels
  It follows Tunnel Amount. While this is on, Pure's own tunnel fog dimmer is forced off (Pure's dimmer is too weak)


BLOOM, GLARE, SUN:
• Exilitay Sun Blinding shader, separate from Peter's sun blinding
• Bloom/glare retuned for day & night
• New glare boost multipliers for day, night, bad weather & foggy weather
• Godrays are cut after sun is below horizon (prevents godrays showing when sun has completely set)


COLOR:
• New color grades (Chroma, Cine Teal, Fuji, Filmic, Kodak, Monaco, Paris)
• Removed: Exilitay Punch, Autumn & NFS
Color profiles
• Day color profiles are slightly warmer to 1.09
• Exilitay-Spec color temp becomes slightly warmer at lower sun angles


NIGHT SKYDOMES:
Custom night skydomes (animated/rotating)
• 3 Aurora skies and galaxy sky are now part of the ppfilter
• Adjustments for rotation, brightness, contrast, height, animation speed, and color


FOG:
Fog Light Emissive Glow
• Street lamps fog glow can be controlled in emissives tab (overrides for all weather)
Heavy fog
• Thick fog switches to Exilitay-Style preset automatically
  Custom and No Fog presets aren't affected


APP:
New Lua app - filter controls & presets
• Info: basic information about the app 
• PPFilter: the filter settings. Save, load and reset settings locally
• Presets: 5 factory presets, plus custom ones to save, import, and export
• Settings: window opacity, window size presets, tooltips, and more
• Images: Preview images for Night Skydomes, Colorgrades & Presets
License
• The ppfilter stays inactive until you activate the app
• Reveal your key on My Account, then paste it into the app
• One device at a time. Reset your key from My Account (every 30 days)


OTHER CHANGES & BUG FIXES
• Glare: GT7-style preset is renamed to Star 
• Bloom radius slider for day & night
• Black Limit Low/High are now Black Point Day and Black Point Night
• Forced Pure Planets off to fix strong glare in night sky (the moon stays)
• No Fog is a new fog style preset 
• Lens dirt has a new third overlay and a blend mode adjustment
• New sunblinding shader + separate interior sun blinding
• Custom Occlusion is used instead of Pure's occlusion
• HDR is no longer supported
