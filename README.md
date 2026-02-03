local GameScripts = {
    ["2023680558"] = {
        url = "https://api.jnkie.com/api/v1/luascripts/public/6e89ed0fc5cabc676513be69c347c6f2b3566c1a6547d30202eb7a2bbf9007e7/download"
    },
    ["5909935640"] = {
        url = "https://api.jnkie.com/api/v1/luascripts/public/dcded354e622870c151e87f40c873c1d9387a702ec0c41fc9916c40ff51a237e/download"
    },
    ["5421899973"] = {
        url = "https://api.jnkie.com/api/v1/luascripts/public/c8ae7551adf5c8beeb810ac38549f5d8a95e08f813988e02f8ab8e461ef1f29f/download"
    },
    ["6701277882"] = {
        url = "https://api.jnkie.com/api/v1/luascripts/public/1d7cf9433a4c043fca6f23f0a573742428b7e970a6f5dd4000493892252bf557/download"
    },
    ["7585079192"] = {
        url = "https://api.jnkie.com/api/v1/luascripts/public/0982e25bc5a662039985cc258a0401e9fca50425083acd0f90861c2671d261f9/download"
    },
    ["9266873836"] = {
        url = "https://api.jnkie.com/api/v1/luascripts/public/a18c8cd6892a87814a7464804312acebf86e19b900528a7d8ae1a832c65a1237/download"
    }
}

-- Execute
local detectedGame = GameScripts[tostring(game.GameId)]

if detectedGame then
    loadstring(game:HttpGet(detectedGame.url))()
end
