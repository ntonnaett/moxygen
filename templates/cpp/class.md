## {{kind}} `{{name}}` {{anchor refid}}

{{#if basecompoundref}}
```
{{kind}} {{name}}
  {{#each basecompoundref}}
  : {{prot}} {{name}}
  {{/each}}
```
{{/if}}

{{briefdescription}}

{{detaileddescription}}

### Members

{{#each filtered.compounds}}
#### {{title proto}} {{anchor refid}}

{{briefdescription}}

{{detaileddescription}}
{{/each}}

{{#each filtered.members}}
??? example "{{title proto}} <br/>// {{briefdescription}}"
    {{#if enumvalue}}
     Values                         | Descriptions                                
    --------------------------------|---------------------------------------------
    {{#each enumvalue}}    {{cell name}}            | {{cell summary}}
    {{/each}}
    {{/if}}
    {{detaileddescription}}

{{/each}}
