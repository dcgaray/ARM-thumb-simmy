all:
	g++ -g main.cpp decode.cpp thumbsim_driver.cpp parse.cpp execute.cpp -o thumbsim -w

run:
	./thumbsim -i -s -d -c 256 -f inputs/shang.O0.sim

clean:
	rm -rf ./*.o ./thumbsim
