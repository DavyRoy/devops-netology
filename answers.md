# Ответы на задания

1. Полный хеш и комментарий коммита, хеш которого начинается на aefea:
   - Команда: `git log --oneline | grep ^aefea`
   - Ответ: `aefead2207 Update CHANGELOG.md`

2. Коммит `85024d3` соответствует тегу:
   - Команда: `git tag --contains 85024d3`
   - Ответ: 'v0.12.23, v0.12.24, v0.12.25, v0.12.26, v0.12.27, v0.12.28, v0.12.29, v0.12.30, v0.12.31'

3. Коммит `b8d720` имеет следующих родителей:
   - Команда: `git show --pretty=format:%P b8d720`
   - Ответ: `56cd7859e05c36c06b56d013b55a252d0bb7e158 9ea88f22fc6269854151c571162c5bcf958bee2b`

4. Коммиты между тегами `v0.12.23` и `v0.12.24`:
   - Команда: `git log v0.12.23..v0.12.24 --oneline`
   - Ответ: `33ff1c03bb (tag: v0.12.24) v0.12.24
b14b74c493 [Website] vmc provider links
3f235065b9 Update CHANGELOG.md
6ae64e247b registry: Fix panic when server is unreachable
5c619ca1ba website: Remove links to the getting started guide's old location
06275647e2 Update CHANGELOG.md
d5f9411f51 command: Fix bug when using terraform login on Windows
4b6d06cc5d Update CHANGELOG.md
dd01a35078 Update CHANGELOG.md
225466bc3e Cleanup after v0.12.23 release`

5. Коммит, в котором была создана функция `func providerSource`:
   - Команда: `git log -S 'func providerSource' --pretty=format:%H -p`
   - Ответ: `5af1e6234ab6da412fb8637393c5a17a1b293663`

6. Коммиты, в которых изменялась функция `globalPluginDirs`:
   - Команда: `git log -S 'globalPluginDirs' --pretty=format:%H -p`
   - Ответ:`65c4ba736375607b6af6c035972f7f151232b6c6
125eb51dc40b049b38bf2ed11c32c6f594c8ef96
22c121df8631c4499d070329c9aa7f5b291494e1
7c7e5d8f0a6a50812e6e4db3016ebfd36fa5eaef
35a058fb3ddfae9cfee0b3893822c9a95b920f4c'

7. Автор функции `synchronizedWriters`:
   - Команда: `git log -S 'func synchronizedWriters' --pretty=format:%H -p`
   - Ответ: `bdfea50cc85161dea41be0fe3381fd98731ff786`
