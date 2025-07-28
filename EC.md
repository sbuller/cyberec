devices:

	Battery Monitor
	Battery Charger
	USB-PD controller

	Main System Power Supply
	Network Power Supply?
	Suspend mode power supply?
	RTC

	supplies for other peripherals?

	fan(s)

radios:
	mavlink (mlrs)
	elrs
	video (composite) ?MHz
	video (digital) ?
	other?

busses:
	i2c/smbus/pmbus may need to be split:
		battery monitor
		battery charger
		usb-pd controller
		host
		compass?
		
	uart (not so much a bus, as individual connections):
		gps
		router
		host
		switch?

	mdio:
		switch & other PHYs

	other:
		gps pps
		switch
		usb?
