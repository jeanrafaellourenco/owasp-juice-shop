# P-R-E-R-I-G-O ☠️

Modo inseguro : 

Se definido como `disabled`, isso ativa todos os desafios potencialmente perigosos, independentemente dos danos que possam causar ao serem executados em um ambiente conteinerizado.
Se definido como `auto`, o modo de segurança é ativado caso o Juice Shop considere que está sendo executado em um ambiente de produção (que tem mais chances de estar exposto ao tráfego da internet).

☠️ Use por sua conta e risco!

```yaml
challenges:
  safetyMode: disabled
```

**Esta configuração não é recomendada em ambiente web mesmo em containers** e por padrão vem configurado como `auto` no arquivo de configuração [lovestickersnerd.yml](lovestickersnerd.yml)

Ao desativar esta opção definindo como `auto`, alguns desafios não estarão mais disponíveis como `Stored XSS` e algumas falhas `SQL`.