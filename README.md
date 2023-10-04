### 全国省市区三级数据库,三级联动地区数据库

格式如下
```
DROP TABLE IF EXISTS `area`;
CREATE TABLE `area`  (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `pid` int(11) UNSIGNED NOT NULL,
  `name` varchar(500) CHARACTER SET utf8 COLLATE utf8_general_ci NOT NULL,
  `visible` tinyint(4) UNSIGNED NOT NULL,
  `displayorder` int(11) UNSIGNED NOT NULL,
  `level` tinyint(3) UNSIGNED NOT NULL,
  PRIMARY KEY (`id`) USING BTREE,
  INDEX `parentId`(`pid`) USING BTREE
) ENGINE = InnoDB AUTO_INCREMENT = 990101 CHARACTER SET = utf8 COLLATE = utf8_general_ci ROW_FORMAT = Compact;

-- ----------------------------
-- Records of area
-- ----------------------------
INSERT INTO `area` VALUES (110000, 0, '北京市', 2, 0, 1);
INSERT INTO `area` VALUES (110100, 110000, '北京市', 2, 0, 2);
INSERT INTO `area` VALUES (110101, 110100, '东城区', 2, 0, 3);
INSERT INTO `area` VALUES (110102, 110100, '西城区', 2, 0, 3);
INSERT INTO `area` VALUES (110103, 110100, '崇文区', 2, 0, 3);
INSERT INTO `area` VALUES (110104, 110100, '宣武区', 2, 0, 3);
INSERT INTO `area` VALUES (110105, 110100, '朝阳区', 2, 0, 3);
INSERT INTO `area` VALUES (110106, 110100, '丰台区', 2, 0, 3);
INSERT INTO `area` VALUES (110107, 110100, '石景山区', 2, 0, 3);
INSERT INTO `area` VALUES (110108, 110100, '海淀区', 2, 0, 3);
INSERT INTO `area` VALUES (110109, 110100, '门头沟区', 2, 0, 3);
INSERT INTO `area` VALUES (110111, 110100, '房山区', 2, 0, 3);
INSERT INTO `area` VALUES (110112, 110100, '通州区', 2, 0, 3);
INSERT INTO `area` VALUES (110113, 110100, '顺义区', 2, 0, 3);
INSERT INTO `area` VALUES (110114, 110100, '昌平区', 2, 0, 3);
INSERT INTO `area` VALUES (110115, 110100, '大兴区', 2, 0, 3);
INSERT INTO `area` VALUES (110116, 110100, '怀柔区', 2, 0, 3);
INSERT INTO `area` VALUES (110117, 110100, '平谷区', 2, 0, 3);
INSERT INTO `area` VALUES (110228, 110200, '密云县', 2, 0, 3);
INSERT INTO `area` VALUES (110229, 110200, '延庆县', 2, 0, 3);
INSERT INTO `area` VALUES (110230, 110100, '其它区', 2, 0, 3);
```
