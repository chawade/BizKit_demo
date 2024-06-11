<template>
    <section class="stock-adjustment">
        <div class="container">
            <h3>สร้าง/แก้ไข การปรับสต๊อก</h3>
            <div class="breadcrumb">
                <p>หน้าแรก > ปรับสินค้า > สร้าง/แก้ไข การปรับสต๊อก</p>
            </div>
            <div class="form">
                <h5><span>สร้าง/แก้ไข การปรับสต๊อก</span></h5>
                <div class="form-section">
                    <div class="form-l">
                        <div class="form-group">
                            <label>เลขที่การปรับสินค้า</label>
                            <input type="text" placeholder="--ออกโดยระบบ--" disabled />
                        </div>
                        <div class="form-group">
                            <label>คลังสินค้า</label>
                            <select>
                                <option value="">เลือก</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <label>ผู้รับผิดชอบ</label>
                            <select>
                                <option value="">เลือก</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <label>หมายเหตุ</label>
                            <textarea></textarea>
                        </div>
                    </div>
                    <div class="form-r">
                        <div class="form-group">
                            <label>วันที่ออกเอกสาร</label>
                            <input type="date" />
                        </div>
                        <div class="form-group">
                            <label>การปรับสินค้า</label>
                            <select>
                                <option value="">เลือก</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <label>หมายเลขอ้างอิง</label>
                            <input type="text" />
                        </div>
                    </div>
                </div>
                <div class="product-list">
                    <h3>รายการสินค้า</h3>
                    <table>
                        <thead>
                            <tr>
                                <th>ลำดับ</th>
                                <th>รูป</th>
                                <th>รหัสสินค้า</th>
                                <th>ชื่อสินค้า</th>
                                <th>เลขล็อต/ซีเรียล</th>
                                <th>วันหมดอายุ</th>
                                <th>ไลเคชั่น-ชั้น</th>
                                <th>คงเหลือ</th>
                                <th>พร้อมใช้</th>
                                <th>จำนวนที่ปรับ</th>
                                <th>หน่วย</th>
                                <th>ราคา</th>
                                <th>หมายเหตุ</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <td></td>
                                <td></td>
                                <td></td>
                                <td></td>
                                <td></td>
                                <td></td>
                                <td></td>
                                <td></td>
                                <td></td>
                                <td></td>
                                <td></td>
                                <td></td>
                                <td></td>
                            </tr>
                        </tbody>
                    </table>
                    <div class="action-new">
                        <button @click="addProduct" class="btn-primary">เพิ่มสินค้า</button>
                    </div>
                </div>
            </div>
            </div>
                <div class="actions">
                    <button @click="save" class="btn-primary">บันทึก</button>
                    <button @click="saveAndApprove" class="btn-primary">บันทึกและอนุมัติ</button>
                    <button @click="cancel" class="btn-danger">ยกเลิก</button>
                </div>
    </section>
</template>

<style scoped>
.breadcrumb p {
    margin: 10px 0;
    background-color: var(--color-white);
    color: #6c757d;
    padding: 12px;
    border-radius: 5px;
}

.form {
    background-color: var(--color-white);
    padding: 20px;
    border-radius: 5px;
    margin-bottom: 20px;
}

.form-section {
    display: grid;
    grid-template-columns: 50% auto;
    gap: 5rem;
}

.form-group {
    display: flex;
    margin-bottom: 15px;
}

.form-group label {
    display: block;
    /* font-weight: 600; */
    margin-left: 0;
}

.form-group input,
.form-group select,
.form-group textarea {
    width: 70%;
    padding: 8px;
    border: 1px solid #ced4da;
    border-radius: 4px;
    font-size: 1rem;
}

.product-list {
    margin-bottom: 20px;
}

.product-list h4 {
    margin-bottom: 10px;
    font-weight: 700;
}

.product-list table {
    width: 100%;
    border-collapse: collapse;
    margin-bottom: 10px;
}

.product-list th,
.product-list td {
    border: 1px solid #dee2e6;
    padding: 10px;
    text-align: center;
}

.product-list th {
    /* background-color: #e9ecef; */
    font-weight: 700;
}

.action-new {
    display: flex;
    justify-content: end;
}

.actions {
    display: block;
        position: fixed;
        bottom: 0;
        width: 100%;
        background: var(--color-white);
        display: flex;
        gap: 12px;
        z-index: 11;
        padding: .5rem 1rem;
        justify-content: end;
}
</style>