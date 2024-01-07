- 👋 Hi, I’m @Bloxfruitsisthegoat
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Bloxfruitsisthegoat/Bloxfruitsisthegoat is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
local Old
Old = hookfunction(request, newcclosure(function(a, b)
    if type(a) == "table" then
        for i, v in pairs(a) do
            if i == "Url" and v == 'https://btteam.net/checkpoint/check.php' then
                return {
                    StatusCode = 200,
                    Body = 'lol'
                }
            elseif i == "Url" and v == 'https://btteam.net/checkpoint/verify.php?h=lol&k=Cracked' then
                return {
                    StatusCode = 200,
                    Body = '{"status":"success","message":"VALID_KEY"}'
                }
            end
        end
    end
    return Old(a, b)
end))
loadstring(game:HttpGet('https://btteam.net/scripts-auth/', true))()

![Screenshot_20240108-072140_YouTube](https://github.com/Bloxfruitsisthegoat/Bloxfruitsisthegoat/assets/155919779/139d533b-1319-4328-ba7d-62ebd1ad73cc)
