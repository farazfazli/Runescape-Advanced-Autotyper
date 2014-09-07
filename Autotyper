# Written by: Faraz Fazli
tell application "System Events"
	set x to 1
	set b to 1
	display dialog "Text:" default answer ""
	set qtext to the text returned of the result
	display dialog "# of times:" default answer "10"
	set numberoftimes to the text returned of the result
	display dialog "Speed (1-4):" default answer "2"
	set rapidity to the text returned of the result
	if rapidity = 1 then
		set b to 7
	end if
	if rapidity = 2 then
		set b to 5
	end if
	if rapidity = 3 then
		set b to 3
	end if
	if rapidity = 4 then
		set DelayShort to 1.2
		set DelayLong to 1.7
	end if
	if rapidity ≠ 4 then
		set TxtCount to count (qtext)
		set a to TxtCount * 0.2
		set DelayShort to a + b
		set DelayLong to a + b + (random number from 1 to 2)
	end if
	delay 2
	repeat
		set MovementNum to random number from 1 to 3
		if MovementNum = 1 then
			set Movement to "wave:"
		end if
		if MovementNum = 2 then
			set Movement to "wave2:"
		end if
		if MovementNum = 3 then
			set Movement to "shake:"
		end if
		set EffectNum to random number from 1 to 7
		if EffectNum = 1 then
			set Effect to "cyan:"
		end if
		if EffectNum = 2 then
			set Effect to "green:"
		end if
		if EffectNum = 3 then
			set Effect to "white:"
		end if
		if EffectNum = 4 then
			set Effect to "purple:"
		end if
		if EffectNum = 5 then
			set Effect to "glow1:"
		end if
		if EffectNum = 6 then
			set Effect to "glow2:"
		end if
		if EffectNum = 7 then
			set Effect to "glow3:"
		end if
		x = x + 1
		keystroke Effect & Movement & qtext
		keystroke return
		delay (random number from DelayShort to DelayLong)
		if x = numberoftimes then
			exit repeat
		end if
	end repeat
end tell
end
