- 👋 Hi, I’m @nchaud200
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
nchaud200/nchaud200 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
from Calculate import DataResult


def main():
    print("\n")
    print("To close program Enter 'Exit'")
    file = input("Enter name of file: ") + ".csv".lower()
    print("\n")
    if file == "exit.csv" or file == "Exit.csv":
        exit()
    else:
        DataResult(file)
        try:
            DataResult(file)
            main()
        except Exception as e:
            print(e, "\n")
            print(" - Please Try Again - ")
            main()


if __name__ == "__main__":
    main()
