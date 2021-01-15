ALTER TABLE `sgmp`.`tm_warehouse_group` 
ADD COLUMN  `CODEX` VARCHAR(20) NULL DEFAULT NULL COMMENT '库区精度' ,
ADD COLUMN  `CODEY` VARCHAR(20) NULL DEFAULT NULL COMMENT '库区纬度' ;

UPDATE `sgmp`.`tm_warehouse_group` SET `CODEX` = '108.093491', `CODEY` = '34.273695' WHERE (`GROUP_ID` = '1');
UPDATE `sgmp`.`tm_warehouse_group` SET `CODEX` = '108.148369', `CODEY` = '34.307189' WHERE (`GROUP_ID` = '2');



ALTER TABLE `sgmp`.`tm_warehouse` 
ADD COLUMN `CWC` DOUBLE NULL COMMENT '仓外长' AFTER `IS_DELETED`,
ADD COLUMN `CWK` DOUBLE NULL COMMENT '仓外宽' AFTER `CWC`,
ADD COLUMN `CWYG` DOUBLE NULL COMMENT '仓外檐高' AFTER `CWK`,
ADD COLUMN `CWDG` DOUBLE NULL COMMENT '仓外顶高' AFTER `CWYG`;


use sgmp;
update tm_warehouse  set CWC=36.63,CWK=24,CWYG=7.8,CWDG=10.2
WHERE CODE like 'P%';

update tm_warehouse  set CWC=30,CWK=36,CWYG=8.1,CWDG=10.8
WHERE CODE>='P15' AND CODE<='P17';

update tm_warehouse  set CWC=36.78,CWK=24.24,CWYG=9,CWDG=11.4
WHERE CODE in ('P18','P19','P20','P21','P22','P23' );

update tm_warehouse  set CWC=22,CWK=0,CWYG=23.75,CWDG=28.5
WHERE CODE>='Q1' AND CODE<='Q8';

update tm_warehouse  set CWC=30.25,CWK=28.8,CWYG=6.9,CWDG=12.3
WHERE CODE like '武功分库%';
commit;
