TARGET = radar_basic

all: $(TARGET)

radar_basic:		main.o pulse_train.o range_resolution.o doppler_frequency.o radar_range_equation.o power_aperture.o math_tech.o
	$(CC) -o radar_basic main.o math_tech.o pulse_train.o range_resolution.o doppler_frequency.o radar_range_equation.o power_aperture.o -lm

pulse_train:		pulse_train.o
	$(CC) -c pulse_train.c

range_resolution:	range_resolution.o
	$(CC) -c range_resolution.c

doppler_frequency:	doppler_frequency.o
	$(CC) -c doppler_frequency.c

radar_range_equation:	radar_range_equation.o
	$(CC) -c radar_range_equation.c

power_aperture:		power_aperture.o
	$(CC) -c power_aperture.c

math_tech:		math_tech.o
	$(CC) -c math_tech.c

clean:
	rm -rf $(TARGET)
	rm -rf *.o