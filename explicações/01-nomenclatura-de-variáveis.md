// Nomeclatura de variáveis

const users = ['Giovanna', 'Gabriel', 'Luanna']


// ❌ errado
const filtered = users.filter(u => {
  return u.startsWith('G')
})

// ✅ certo
const usersStartingWithLetterG = users.filter(u => {
  return u.startsWith('G')
})

// evite nomes genéricos (data, response, params, list, args)

// ❌ errado
function getUsers() {
  const data = getUsersFromDataBase()

  return data
}

// ✅ certo
function getUsers() {
  const users = getUsersFromDataBase()

  return users
}