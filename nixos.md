## Установка на NixOS

Добавить пакет `anilibria-winmaclinux` в список пакетов:

* Общесистемно:

    ```nix
    environment.systemPackages = with pkgs; [ anilibria-winmaclinux ];
    ```

* Для определенного пользователя (в примере имя пользователя - bob)

    ```nix
    users.users.bob.packages = with pkgs; [ anilibria-winmaclinux ];
    ```

### Как найти приложение?

Приложение будет доступно из меню и в терминале по имени AniLibria.

### Как обновить приложение?

Программа будет обновляться вместе с OS.

[Раздел документации про обновление NixOS](https://nixos.org/manual/nixos/unstable/#sec-upgrading)
